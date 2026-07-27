---
id: ROT-consultas-contas-pagas
title: "Consultas Contas Pagas"
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
  - from: Consultas Contas Pagas
    type: RELACIONA_COM
    to: Movimentos Liquidação Em Lote
  - from: Consultas Contas Pagas
    type: RELACIONA_COM
    to: Movimentos Liquidação Individual
---

## Visão Geral
Consulta os documentos já liquidados (pagos) para o fornecedor, filtrando por período.

## Quem Usa
Setor Financeiro, responsável pelas contas a pagar.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/business

## Como Usar (passo a passo)
1. Acessar **Consultas » Contas Pagas**, ou pelo ícone direto na barra de ferramentas.

## Campos e Parâmetros Importantes
Sem dúvidas — rotina simples de gerar.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- Movimentos Liquidação (Em Lote, Individual, com Cheques Pré Recebidos) — as liquidações de documentos a pagar.
