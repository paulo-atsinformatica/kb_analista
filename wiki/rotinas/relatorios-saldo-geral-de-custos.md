---
id: ROT-relatorios-saldo-geral-de-custos
title: "Relatórios Saldo Geral de Custos"
type: rotina
audience: all
modulos: ["windows/caixa", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Relatórios Saldo Geral de Custos
    type: RELACIONA_COM
    to: Cadastro Centro de Custo
  - from: Relatórios Saldo Geral de Custos
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
---

## Visão Geral
Mostra os saldos gastos de acordo com o centro de custo, para identificar em qual área da empresa estão sendo gerados os maiores gastos.

## Quem Usa
Financeiro/Administrativo.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Relatório de Saldo Geral de Custos**.
2. Informar Filial, Período, Centro de Custo.
3. Escolher Tipo de Relatório (Sintético ou Analítico) e pesquisar por data de Pagamento ou Emissão.

## Campos e Parâmetros Importantes
Rotina simples — apenas informar os dados.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/cadastro-centro-de-custo|Cadastro Centro de Custo]]
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
