---
id: ROT-fluxo-de-caixa
title: "Fluxo de Caixa"
type: rotina
audience: all
modulos: ["windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Fluxo de Caixa
    type: RELACIONA_COM
    to: Contas a Pagar
  - from: Fluxo de Caixa
    type: RELACIONA_COM
    to: Contas a Receber
---

> [!NOTE] Correção de módulo
> Pré-mapeada originalmente em `windows/bancos` e `windows/caixa`. Confirmado com o analista que essa rotina **só existe no Resulth Business** (`windows/business`) — não aparece em Windows » Caixa nem Windows » Bancos.

## Visão Geral
Consulta o fluxo de Contas a Receber (inclusive pré-recebidos) e Contas a Pagar (inclusive pré-emitidos), com filtros por dia, movimentação, mês/ano e tipo de documento.

## Quem Usa
Dono da empresa (para observar entradas e saídas) e setor Financeiro.

## Módulos onde esta rotina existe
- windows/business

## Como Usar (passo a passo)
1. Acessar **Consultas » Caixa » Fluxo de Caixa** (no sistema Resulth Business).
2. Filtrar por Filial, Tipo de Documento, Moeda e Mês/Ano.
3. Escolher se deseja considerar Cheques Pré-Datados e Cheques Pré-Recebidos.
4. Visualizar o total por dia no calendário do mês; duplo-clique numa data para mais detalhes.

## Campos e Parâmetros Importantes
Sem dúvidas registradas sobre os filtros.

## Erros Comuns / Pontos de Atenção
Sem erros — rotina usada apenas para consulta. Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- Contas a Pagar
- Contas a Receber
