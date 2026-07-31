---
id: ROT-movimentos-geracao-de-previsoes
title: "Movimentos Geração de Previsões"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Movimentos Geração de Previsões
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
  - from: Movimentos Geração de Previsões
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
---

## Visão Geral
Gera/consulta os valores que vão vencer para pagamento. Serve apenas para consulta, não movimenta nada.

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Movimentos » Geração de Previsões**.
2. Informar o Período de análise, a(s) Filial(is), Mês/Ano final, e Dia de vencimento.
3. Selecionar uma ou todas as contas caixa.
4. Informar o Tipo de Documento (usado apenas para previsão de contas a pagar) e o Fornecedor.
5. Clicar em Gerar Previsões.

## Campos e Parâmetros Importantes
Sem dúvidas — rotina simples de utilizar.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
