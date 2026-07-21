---
id: ROT-movimentos-fechamento-de-caixa-financeiro
title: "Movimentos Fechamento de Caixa Financeiro"
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
  - from: Movimentos Fechamento de Caixa Financeiro
    type: RELACIONA_COM
    to: Abertura de Caixa
  - from: Movimentos Fechamento de Caixa Financeiro
    type: RELACIONA_COM
    to: Fechamento de Caixa
  - from: Movimentos Fechamento de Caixa Financeiro
    type: RELACIONA_COM
    to: Cadastro de Turnos
  - from: Movimentos Fechamento de Caixa Financeiro
    type: RELACIONA_COM
    to: Lançamentos Avulsos de Caixa
---

## Visão Geral
Rotina usada para fazer a conferência diária do caixa — mostra todas as vendas feitas, lançamentos, formas de pagamento usadas, sangrias/suprimentos feitos, e o valor em dinheiro. É o processo que o operador do caixa faz ao final do turno. Só é possível abrir um novo caixa (de um novo dia) para o operador depois que esse fechamento financeiro for feito.

## Quem Usa
Operador do caixa, e setor administrativo.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Fechamento de Caixa Financeiro**.

## Campos e Parâmetros Importantes
- Diferente do Fechamento de Caixa comum (que permite reabertura), o **Fechamento de Caixa Financeiro é definitivo** — uma vez fechado, não pode mais ser reaberto. Atenção redobrada para informar os valores corretamente antes de confirmar.

## Erros Comuns / Pontos de Atenção
- Vendas/lançamentos que não integraram ao caixa — ocorre quando a operação usada na venda não está marcada para integrar com o caixa, ou está marcada incorretamente (integra quando não deveria), ou algum valor foi lançado errado.
- Sempre informar os valores corretamente na hora do fechamento, para evitar divergências (lembrando que esse fechamento é definitivo).

## Rotinas Relacionadas
- [[rotinas/abertura-de-caixa|Abertura de Caixa]]
- [[rotinas/fechamento-de-caixa|Fechamento de Caixa]]
- [[rotinas/_compartilhadas/cadastro-turnos|Cadastro de Turnos]]
- [[rotinas/lançamentos-avulsos-caixa|Lançamentos Avulsos de Caixa]]
