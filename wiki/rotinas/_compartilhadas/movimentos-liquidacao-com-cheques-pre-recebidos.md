---
id: ROT-movimentos-liquidacao-com-cheques-pre-recebidos
title: "Movimentos Liquidação com Cheques Pré Recebidos"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/contas-a-receber", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Movimentos Liquidação com Cheques Pré Recebidos
    type: RELACIONA_COM
    to: Movimentos Liquidação Em Lote
---

## Visão Geral
Faz a liquidação de documentos a pagar em lote, mas é a única que permite as formas de pagamento **cheque** e **cartão** (a forma "aproveitamento de crédito" é da rotina [[rotinas/_compartilhadas/movimentos-liquidacao-em-lote|Movimentos Liquidação Em Lote]]).

> [!NOTE] Comportamento diferente por módulo
> A mesma rotina, quando acessada pelo módulo **Contas a Receber**, liquida documentos **a receber** em vez de a pagar — o restante do funcionamento é equivalente.

## Quem Usa
Setor Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/contas-a-receber
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Liquidação » Com Cheques Pré Recebidos** (atalho ao lado de Individual, Em Lote e Impressão de Recibos).
2. Informar o Fornecedor (e a Conta Caixa).
3. Selecionar os documentos que serão liquidados na grade superior.
4. Se a forma de pagamento for cheque, informar os dados do cheque na grade "Cheques" da parte inferior da tela; se for outra forma (ex: cartão), informar normalmente nos campos de forma de pagamento.
5. Confirmar a liquidação no botão **Liquidar**.

## Campos e Parâmetros Importantes
_(nenhum ponto específico levantado pelo analista, além do preenchimento da grade de cheques)_

## Erros Comuns / Pontos de Atenção
- Se a liquidação foi feita por esta rotina, o **estorno também deve ser feito por ela mesma** (botão **Estornar** na própria tela) — não pela rotina genérica de Movimentos Estorno, que só funciona para liquidações feitas via Liquidação Individual.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/movimentos-liquidacao-em-lote|Movimentos Liquidação Em Lote]]
