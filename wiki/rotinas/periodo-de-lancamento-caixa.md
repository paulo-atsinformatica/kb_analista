---
id: ROT-periodo-de-lancamento-caixa
title: "Período de Lançamento de Caixa"
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
  - from: Período de Lançamento de Caixa
    type: RELACIONA_COM
    to: Movimentos Inicia Saldo Filiais
  - from: Período de Lançamento de Caixa
    type: RELACIONA_COM
    to: Parâmetros Caixa
---

> [!NOTE] Duplicata mesclada
> Também aparecia no levantamento original como "Movimentos Período de Lançamentos" — mesma rotina, nomes diferentes.

## Visão Geral
Rotina usada apenas para **renovar o período de lançamento** do caixa da filial, quando ele expira. Se o período estiver configurado para atualização automática (via Parâmetros Caixa), essa rotina não é utilizada.

## Quem Usa
Administrativo ou Financeiro, dependendo da regra de negócio de cada empresa.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Período de Lançamentos**.

## Campos e Parâmetros Importantes
- Recomendação: sempre colocar a data final do período com uma margem maior, para evitar que expire com frequência (ver [[rotinas/movimentos-inicia-saldo-filiais|Movimentos Inicia Saldo Filiais]]).

## Erros Comuns / Pontos de Atenção
- Período cadastrado muito curto expira e exige nova renovação manual — evitável configurando atualização automática em Parâmetros Caixa.

## Rotinas Relacionadas
- [[rotinas/movimentos-inicia-saldo-filiais|Movimentos Inicia Saldo Filiais]]
- [[rotinas/parametros-caixa|Parâmetros Caixa]] — pode configurar a renovação automática, dispensando o uso manual desta rotina.
