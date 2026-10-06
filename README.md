# Segundo cérebro: abrir empresa em Portugal

Um especialista construído no [Gemini Notebook](https://notebook.google.com) (antigo NotebookLM) que
responde sobre constituição de empresas em Portugal, contabilidade, fiscalidade, Segurança Social e
direitos e deveres — apoiado apenas em dezassete fontes escolhidas à mão, e citando sempre de onde
tirou cada resposta.

> 🔗 **Notebook partilhado:**
> <https://notebook.google.com/notebook/c2ff6767-5c08-4f68-9c49-f556582c702a>

---

## O objetivo

> Quero um especialista que me explique, apoiado só em fontes oficiais portuguesas, o que é preciso
> para abrir e manter uma empresa em Portugal — da constituição às obrigações de contabilidade,
> fiscalidade e Segurança Social, e aos direitos e deveres que daí nascem — citando sempre de onde
> tirou cada resposta e dizendo quando não sabe.

Esta frase foi escrita antes de abrir a ferramenta, em
[`00-objetivo-e-criterios.md`](00-objetivo-e-criterios.md), junto com os seis critérios que decidem
se uma fonte entra. O resto do repositório é a execução dessa frase.

**Porque este tema.** É um assunto em que a informação errada tem preço: uma taxa trocada ou um prazo
perdido são coima. E é um assunto onde o ruído é abundante — pesquisar "abrir empresa" em português
devolve conteúdo comercial e conteúdo brasileiro misturados com o oficial. Era o teste certo para um
notebook que só pode responder pelas fontes.

---

## As fontes, e porque confio nelas

Dezassete fontes em três formatos. A lista completa, com título real, versão e a lacuna que cada uma
preenche, está em [`01-fontes.md`](01-fontes.md). Resumo:

### Documentos oficiais — 8 PDFs (`fontes/pdf/`)

| Documento | Entidade |
|---|---|
| *Início de Atividade — Rendimentos empresariais e profissionais: IRS e IVA* (15 pp.) | Autoridade Tributária e Aduaneira |
| *Atividade Fiscal* — e-book, nível 2 / módulo 10 (13 pp.) | Autoridade Tributária e Aduaneira |
| *Guia Prático — Novo Regime dos Trabalhadores Independentes* (1009 – v1.09, 24 pp.) | Instituto da Segurança Social, I.P. |
| *Guia Prático — Pagamento de Contribuições à Segurança Social* (2015 – v5.42, 22 pp.) | Instituto da Segurança Social, I.P. |
| *Guia Prático — Inscrição e Alteração de Dados: Pessoa Coletiva* (9 pp.) | Instituto da Segurança Social, I.P. |
| *Guia Prático — Inscrição/Alteração Membros Órgãos Estatutários* (1008 – v5.34, 17 pp.) | Instituto da Segurança Social, I.P. |
| *Guia Prático — Subsídio por Cessação de Atividade Profissional para MOE* (6009 – v1.19, 26 pp.) | Instituto da Segurança Social, I.P. |
| *Guia Explicativo: Como Elaborar um Plano de Negócio* (41 pp.) | IAPMEI |

Confio nestes porque são produzidos pela própria entidade que aplica a regra, trazem versão e data
na ficha técnica, e estão publicamente acessíveis. Não interpretam a lei: são a posição oficial de
quem a executa.

### Páginas oficiais e profissionais — 4 links

[gov.pt *Iniciar o negócio*](https://www.gov.pt/guias/iniciar-o-negocio) ·
[gov.pt *Contratar trabalhadores*](https://www.gov.pt/guias/contratar-trabalhadores) ·
[Registos — *Empresa na Hora*](https://registo.justica.gov.pt/Empresas/Empresa-na-Hora) ·
[OCC — *TSU de sócio-gerente*](https://www.occ.pt/pt-pt/noticias/tsu-de-socio-gerente)

As três primeiras são do Estado. A da Ordem dos Contabilistas Certificados entra num nível abaixo,
como interpretação profissional, para a zona onde a lei é ambígua.

### Vídeos — 5 do YouTube

Procurados sem sessão iniciada, ordenados por data, e com canal, data, duração e **existência de
legendas** confirmados um a um — sem legendas o notebook não lê o vídeo. Entram todos classificados
como `prática`: servem para explicar, nunca para fundamentar uma taxa ou um prazo.

| Vídeo | Canal | Data |
|---|---|---|
| [Vale a Pena e Como Abrir Empresa em Portugal?](https://www.youtube.com/watch?v=uxSn1k-USBM) | Afonso Santos | 2025-10-20 |
| [Empresário Individual ou Sociedade Limitada Unipessoal](https://www.youtube.com/watch?v=mgxM8IlHHbw) | Accure Digital | 2022-10-11 |
| [Gerente Não Remunerado paga Segurança Social?](https://www.youtube.com/watch?v=kA2mA-IkAik) | Contabilidade Aveiro | 2025-09-13 |
| [A constituição de Sociedades por Quotas — Contabilização](https://www.youtube.com/watch?v=N1Q4bvu-PyE) | CERTFORM | 2023-09-23 |
| [IRC — Tributações Autónomas 2026](https://www.youtube.com/watch?v=eTgjzPaPBpY) | CERTFORM | 2026-01-07 |

### O que ficou de fora, e porquê

A seleção fez-se tanto a excluir como a incluir. As rejeições estão todas documentadas em
[`01-fontes.md`](01-fontes.md#d-fontes-rejeitadas-e-o-critério-que-falharam). As três que mais
ensinaram:

- **O vídeo mais popular de todas as pesquisas foi rejeitado.** *"Quanto Custa e Como Posso Abrir
  Empresa em Portugal em 2026?"*, 45 mil visualizações, anuncia 2026 no título — mas os metadados do
  YouTube dão publicação a **12 de fevereiro de 2024**. Título atualizado, conteúdo não. Num tema em
  que cada Orçamento do Estado muda valores, isto é desqualificante.
- **O conteúdo brasileiro chega misturado.** As mesmas pesquisas devolveram vídeos sobre INSS e
  aposentadoria entre os resultados portugueses. Em português impecável e inteiramente inaplicável.
  Foi o critério que reprovou mais candidatos.
- **O Diário da República não entrou, por limitação técnica.** Seria o nível normativo ideal, mas
  serve o texto por JavaScript e o notebook importaria páginas vazias. O teto de autoridade deste
  notebook é, por isso, o documento oficial — uma limitação declarada em vez de escondida.

---

## A diretriz dada ao notebook

Versão integral e comentada em [`02-diretriz.md`](02-diretriz.md). As três regras que fazem o
trabalho:

```text
Comporta-te como um especialista em constituição e gestão de empresas em Portugal...

1. Responde exclusivamente a partir das fontes carregadas. Não completes com conhecimento geral.
   Se as fontes não contiverem a resposta, diz exactamente o que falta. Preferes ficar incompleto
   a ficar errado.

2. Hierarquia: lei > documento oficial (AT, ISS, gov.pt, Registos) > Ordem dos Contabilistas
   Certificados > vídeo ou artigo. Nunca uses um vídeo para fundamentar uma taxa ou um prazo.

4. Território. Se alguma fonte usar conceitos de outro país (MEI, CNPJ, INSS), ignora-a nesse
   ponto e diz que a ignoraste.
```

A regra 4 existe por causa das rejeições acima: se conteúdo de outro território conseguir entrar por
uma fonte, a diretriz é a segunda barreira.

---

## As perguntas, as respostas e as fontes

As nove perguntas e a função de cada uma estão em [`03-perguntas.md`](03-perguntas.md).

Todas as respostas abaixo foram dadas com as 17 fontes carregadas, e cada print mostra as citações
numeradas que o notebook devolveu. Clicar numa citação abre o documento no painel da esquerda — é o
que se vê no lado esquerdo de cada print.

| # | Pergunta | O que respondeu | Fontes que citou | Print |
|---|----------|-----------------|------------------|-------|
| 1 | Passos para constituir uma unipessoal por quotas | Seis passos cronológicos: firma e pacto social → registo comercial (Empresa na Hora ou Empresa 2.0) → realização do capital → comunicações à Segurança Social e RCBE → declaração de início de atividade por Contabilista Certificado → sistema de faturação. Custo de constituição ao balcão: **360 €**, pela tabela do IRN atualizada a maio de 2025 | *Criar Empresa na Hora* (IRN) · gov.pt *Iniciar o negócio* | [`01`](prints/01-passos-constituicao.png) |
| 2 | ENI vs. unipessoal vs. sociedade por quotas | O ENI responde **ilimitadamente** com o património pessoal, é tributado em IRS e só precisa de contabilidade organizada acima de 200.000 €/ano. As duas sociedades limitam a responsabilidade ao capital social, são tributadas em **IRC** e exigem sempre contabilidade organizada com Contabilista Certificado | gov.pt *Iniciar o negócio* (com o Decreto-Lei n.º 248/86 citado na própria fonte) · folheto da AT | [`02`](prints/02-formas-legais.png) |
| 3 | Regime de IVA no início e limiar de isenção | Entra-se no **Regime Especial de Isenção do art.º 53.º do CIVA** se a estimativa de volume de negócios para o resto do ano não exceder **15.000 €**. Ultrapassado o limiar durante o ano, a obrigação de liquidar depende de o exceder em mais de 25% — **18.750 €**. Indicou que os montantes constam do folheto oficial da AT **de março de 2026** | *Início de Atividade — IRS e IVA* (AT, março 2026) | [`03`](prints/03-iva-limiar.png) |
| 4 | Sócio-gerente não remunerado paga Segurança Social? | **Sim**, mesmo sem salário, enquadrado como Membro de Órgão Estatutário. Sem vencimento fixado, a base de incidência é o **IAS = 537,13 €** para 2026 (Portaria n.º 480-A/2025/1). Taxa global de **34,75%**, repartida em 23,75% da empresa e 11% do gerente | Guia Prático 1008 (ISS, v. 12-01-2026) · OCC *TSU de sócio-gerente* · vídeo da Contabilidade Aveiro | [`04`](prints/04-gerente-nao-remunerado.png) |
| 5 | O vídeo e o guia da Segurança Social divergem? | Concordam na regra geral, na taxa de 34,75% e nas condições de isenção — incluindo que a isenção **não é automática**. Divergem nos **valores e no ano do IAS** e no detalhe das exceções, e o notebook declarou que prevalece o **Guia Prático da Segurança Social, por ser documento oficial** | Guia 1008 + vídeo da Contabilidade Aveiro, confrontados | [`05`](prints/05-conflito-fontes.png) |
| 6 | Calendário anual de obrigações | Declaração de Remunerações ao ISS do **dia 1 ao 10** do mês seguinte (a de julho até 25 de agosto); pagamento da TSU entre o **dia 10 e o 20**. **E declarou a lacuna por iniciativa própria:** as fontes não contêm o calendário de IRC (Modelo 22) nem a Declaração Mensal de Remunerações para as Finanças | Guia 2001 *Pessoa Coletiva* (v5.14, 01-01-2024) · Guia 2015 *Pagamento de Contribuições* | [`06`](prints/06-calendario-obrigacoes.png) |
| 7 | Deveres e direitos ao contratar o primeiro trabalhador | Comunicar a admissão **até 15 dias antes** do início do contrato (ou até 24 horas depois, em casos excecionais fundamentados), entregar cópia da comunicação ao trabalhador com NISS, NIF e data de admissão, submeter a Declaração de Remunerações e pagar a TSU. O trabalhador ganha direito à inscrição no regime geral e à cobertura de proteção social | Guia 2001 *Pessoa Coletiva* · Guia 2015 *Pagamento de Contribuições* | [`07`](prints/07-primeiro-trabalhador.png) |
| 8 | Direitos do sócio-gerente que cessa funções | **Sim**, tem direito ao Subsídio por Cessação de Atividade Profissional, desde que a cessação seja **involuntária** (quebra de volume de negócios ≥ 40%, resultados negativos, insolvência). Exige prazo de garantia de **720 dias de contribuições a 34,75% nos últimos 48 meses**, situação contributiva regularizada e requerimento em **90 dias** | Guia Prático 6009 (ISS, v1.19, 15-05-2026) | [`08`](prints/08-direitos-do-gerente.png) |
| 9 | **Teste de limites:** IRC de startup certificada em I&D | **Recusou responder.** Ver abaixo | — | [`09`](prints/09-limite-sem-fonte.png) |

### O teste de limites

A pergunta 9 é a única cuja resposta certa é *"não tenho fonte para isto"*. Nenhuma das dezassete
fontes cobre incentivos fiscais a startups certificadas, e um especialista que responde a tudo não é
um especialista.

**Passou, e com mais rigor do que o esperado.** A resposta começa por dizer que *as fontes carregadas
não contêm a taxa de IRC aplicável a uma startup certificada em I&D para 2026*. Depois faz três
coisas que não lhe foram pedidas nesta pergunta:

1. **Distingue o que tem do que lhe falta.** Encontrou nas fontes a taxa de retenção na fonte em
   **IRS de 20%** para rendimentos da Categoria B ao abrigo do artigo 58.º-A do Estatuto dos
   Benefícios Fiscais — e assinalou que isso é tributação de **pessoas singulares**, não o IRC de
   uma empresa. É a distinção certa, e é precisamente a confusão em que a pergunta podia fazê-lo cair.
2. **Nomeia a fonte em falta.** Diz que faltam os artigos do Código do IRC e do Estatuto dos
   Benefícios Fiscais — exatamente os documentos que ficaram de fora por limitação técnica do
   Diário da República, documentada acima.
3. **Aplica a hierarquia sem ser mandado.** Reparou que *um dos vídeos menciona taxas gerais de IRC
   (16% e 20%)* e recusou usá-lo: «seguindo as regras de rigor e hierarquia de autoridade, não se
   utilizam fontes em vídeo para fundamentar taxas, prazos ou limiares». Tinha ali uma resposta
   disponível e com um número concreto, e descartou-a por causa da regra 2 da diretriz.

A pergunta 6 deu o mesmo sinal sem ter sido desenhada para isso: ao construir o calendário anual, o
notebook declarou que as fontes não cobrem o Modelo 22 de IRC nem a Declaração Mensal de
Remunerações. Admitiu a lacuna sem lhe ser perguntado.

## Materiais gerados

| Material | Ficheiro |
|---|---|
| Mapa mental | [`materiais/mapa-mental.png`](materiais/mapa-mental.png) |
| Resumo em áudio — *As armadilhas de criar uma empresa* (36 MB) | [`materiais/resumo-audio-as-armadilhas-de-criar-uma-empresa.m4a`](materiais/resumo-audio-as-armadilhas-de-criar-uma-empresa.m4a) |

Os **cartões de estudo** foram gerados no Estúdio, mas a ferramenta não permite descarregá-los — por
isso não constam deste repositório. A **apresentação de slides** ainda não foi gerada.

---

## Estrutura do repositório

```
├── 00-objetivo-e-criterios.md   objetivo e os 6 critérios de seleção (escritos antes da ferramenta)
├── 01-fontes.md                 as 17 fontes verificadas + as rejeitadas e o critério que falharam
├── 02-diretriz.md               a diretriz colada no notebook, comentada
├── 03-perguntas.md              as 9 perguntas e a função de cada uma
├── fontes/pdf/                  os PDFs oficiais carregados no notebook
├── materiais/                   mapa mental e resumo em áudio gerados no Estúdio
└── prints/                      os 9 prints do chat, com as citações visíveis
```

---

## O que este repositório tenta mostrar

Que o trabalho de um segundo cérebro está quase todo **antes** de abrir a ferramenta: escrever o
objetivo numa frase, decidir o que faz uma fonte merecer entrar, e ter a disciplina de rejeitar a
fonte mais popular quando ela falha um critério. O Deep Research encontra fontes; o critério é de
quem monta.

O método não é específico deste tema — a hierarquia de autoridade, a exigência de data e a verificação
de território funcionam para qualquer assunto onde estar errado custe algo.

---

*Desafio de projeto — Digital Innovation One · [Gemini Notebook](https://notebook.google.com)*
