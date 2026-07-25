---
id: ROT-relatorios-saldo-contas-sintetico
title: "Relatórios Saldo Contas Sintético"
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
  - from: Relatórios Saldo Contas Sintético
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
  - from: Relatórios Saldo Contas Sintético
    type: RELACIONA_COM
    to: Relatórios Saldo Contas Analítico
---

## Visão Geral
Mesma família do [[rotinas/relatorios-saldo-contas-analitico|Relatórios Saldo Contas Analítico]], mas com mais formas de gerar o relatório: filtro por Filial, Conta Caixa, Período, opção de mostrar saldo de bancos, filtrar por centro de custo, e imprimir subtotais de conta caixa (Sem Subtotais, Nível 1, Nível 2, ou Nível 1 e 2).

## Quem Usa
Setor administrativo/financeiro, para consulta.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Relatório de Saldo de Contas » Sintético**.
2. Informar Filial, Conta Caixa, Período.
3. Opcionalmente: marcar para mostrar saldo de bancos, filtrar por centro de custo, e escolher o nível de subtotal.

## Campos e Parâmetros Importantes
Sem dúvidas registradas.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
- [[rotinas/relatorios-saldo-contas-analitico|Relatórios Saldo Contas Analítico]]
