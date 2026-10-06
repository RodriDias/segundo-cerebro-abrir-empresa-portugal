# Passo 0 — Objetivo e critérios (escrito antes de abrir a ferramenta)

> Este é o "bloco de notas" que o desafio pede que exista **antes** de tocar no Gemini Notebook.
> Nada entra no notebook sem passar pelos critérios abaixo.

## O objetivo, numa frase

> **Quero um especialista que me explique, apoiado só em fontes oficiais portuguesas, o que é
> preciso para abrir e manter uma empresa em Portugal — da constituição às obrigações de
> contabilidade, fiscalidade e Segurança Social, e aos direitos e deveres que daí nascem —
> citando sempre de onde tirou cada resposta e dizendo quando não sabe.**

## O que o segundo cérebro precisa de saber

Cinco blocos, porque são as cinco decisões que uma pessoa real toma por esta ordem:

| # | Bloco | Perguntas que tem de conseguir responder |
|---|-------|------------------------------------------|
| 1 | **Forma legal** | ENI, unipessoal por quotas ou sociedade por quotas? Que responsabilidade, que capital, que custo? |
| 2 | **Constituição** | Empresa na Hora vs. Empresa Online: passos, documentos, prazos, onde se faz |
| 3 | **Fiscalidade** | Início de atividade, enquadramento em IVA e em IRS/IRC, regime simplificado vs. contabilidade organizada, obrigações declarativas e prazos |
| 4 | **Segurança Social** | Trabalhador independente vs. membro de órgão estatutário (sócio-gerente), base de incidência, taxas, isenções, declaração trimestral |
| 5 | **Direitos e deveres** | Como entidade empregadora e como trabalhador: contrato, salário, horários, contabilista certificado obrigatório ou não |

## Critérios para uma fonte entrar

Uma fonte só entra se passar **todos** os seis. Se falhar um, fica fora — mesmo que seja bem escrita.

1. **Hierarquia de autoridade.** Classifico cada fonte em quatro níveis: `normativo` (códigos e
   leis), `oficial` (AT, Segurança Social, gov.pt, Registos), `profissional` (Ordem dos
   Contabilistas Certificados) e `prática` (contabilistas, imprensa especializada). Uma fonte de
   nível inferior nunca pode ser a base para afirmar uma regra que um nível superior define — serve
   para explicar, não para fundamentar.
2. **Datada e versionada.** O documento diz quando foi publicado ou que versão é. Neste tema isto
   não é detalhe: a fiscalidade muda todos os anos com o Orçamento do Estado e as contribuições
   acompanham o IAS. Fonte sem data = fonte que não sei se ainda é verdade.
3. **Verificável no original.** URL público, sem login e sem paywall. Tem de ser possível clicar na
   citação e cair no documento.
4. **Portuguesa, de Portugal.** O critério que mais fontes reprova neste tema. "Abrir empresa",
   "contabilidade" e "segurança social" trazem uma enxurrada de conteúdo brasileiro — MEI, CNPJ,
   Simples Nacional, INSS — em português perfeito e completamente inaplicável. Qualquer fonte que
   fale de INSS ou CNPJ é descartada à cabeça.
5. **Interesse declarado.** Guias de empresas de contabilidade e de software de faturação são úteis
   e estão escritos para humanos, mas existem para vender um serviço. Entram marcadas como `prática`
   e nunca sozinhas num assunto — só a acompanhar a fonte oficial equivalente.
6. **Preenche uma lacuna.** Cada fonte tem de responder a algo que as outras não respondem. Dez
   artigos a dizer o mesmo não são dez fontes, são ruído que dilui as citações.

## Como vou testar se funcionou

O notebook passa se, em todas as perguntas do [passo 3](03-perguntas.md):

- cada afirmação com números (taxas, prazos, limiares) vier com citação clicável;
- a citação apontar para uma fonte de nível `normativo` ou `oficial`, não para um blog;
- numa pergunta deliberadamente fora do âmbito, ele disser que não tem fonte em vez de inventar.
