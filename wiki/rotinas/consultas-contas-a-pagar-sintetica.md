---
id: ROT-consultas-contas-a-pagar-sintetica
title: "Consultas Contas a Pagar Sintética"
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
  - from: Consultas Contas a Pagar Sintética
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Analítica
  - from: Consultas Contas a Pagar Sintética
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Saldos
  - from: Consultas Contas a Pagar Sintética
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Consulta os documentos a pagar de forma simplificada, agrupado por data de vencimento (Vencidos, A Vencer, Total).

## Quem Usa
Setor Financeiro, contas a pagar.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Consultas » Contas a Pagar » Sintética** (atalho Ctrl+S).

## Campos e Parâmetros Importantes
Sem dúvidas — rotina simples.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- Consultas Contas a Pagar Analítica
- Consultas Contas a Pagar Saldos
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
