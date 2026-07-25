---
id: ROT-relatorios-saldo-contas-analitico
title: "Relatórios Saldo Contas Analítico"
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
  - from: Relatórios Saldo Contas Analítico
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
  - from: Relatórios Saldo Contas Analítico
    type: RELACIONA_COM
    to: Relatórios Saldo Contas Sintético
---

## Visão Geral
Relatório detalhado (analítico) dos lançamentos por conta caixa — mostra cada lançamento (data, histórico, valor) com totalização por conta, de forma simplificada para facilitar o entendimento.

## Quem Usa
Setor administrativo/financeiro, para consulta.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Relatório de Saldo de Contas » Analítico**.

## Campos e Parâmetros Importantes
Sem dúvidas registradas.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
- Relatórios Saldo Contas Sintético — mesma família, com mais opções de filtro/geração.
