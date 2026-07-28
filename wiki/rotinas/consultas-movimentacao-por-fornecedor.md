---
id: ROT-consultas-movimentacao-por-fornecedor
title: "Consultas Movimentação Por Fornecedor"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Consultas Movimentação Por Fornecedor
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
  - from: Consultas Movimentação Por Fornecedor
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Analítica
  - from: Consultas Movimentação Por Fornecedor
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Sintética
---

## Visão Geral
Consulta todas as movimentações (entradas de documento, liquidações, D/C) para um fornecedor no período informado.

## Quem Usa
Setor Financeiro / contas a pagar.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/business

## Como Usar (passo a passo)
1. Acessar **Consultas » Movimentação Por Fornecedor** (atalho Ctrl+M).

## Campos e Parâmetros Importantes
Rotina intuitiva: informar o Fornecedor, o Tipo do Movimento (opcional — deixar em branco traz todos) e o Período.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- Consultas Contas a Pagar Analítica
- Consultas Contas a Pagar Sintética
