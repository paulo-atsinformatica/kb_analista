---
id: ROT-movimentos-prorrogacao
title: "Movimentos Prorrogação"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/contas-a-receber", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Movimentos Prorrogação
    type: RELACIONA_COM
    to: Movimentos Entrada de Documento Simples
  - from: Movimentos Prorrogação
    type: RELACIONA_COM
    to: Movimentos Liquidação Em Lote
---

## Visão Geral
Rotina utilizada para prorrogar a data de vencimento de um documento a pagar individual (um documento por vez); também permite alterar o valor do documento.

> [!NOTE] Comportamento diferente por módulo
> No módulo **Contas a Receber**, a rotina equivalente pré-mapeada como "Movimentos Prorrogação Individual" trata documentos **a receber** gerados para clientes, em vez de documentos a pagar gerados para fornecedores.

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/contas-a-receber
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Prorrogação**.
2. Informar o Fornecedor e buscar o documento (Tipo de Doc. e Nº Documento, ou selecionar na grade).
3. Informar o Novo Valor e/ou a Nova Data de Vencimento.
4. Clicar em **Ok** para confirmar — o documento é alterado.

## Campos e Parâmetros Importantes
Rotina simples, sem pontos de atenção relevantes segundo o analista.

## Erros Comuns / Pontos de Atenção
Tranquila, sem erros — [[procedimentos/erros-apenas-por-versao-com-problema|problemas só ocorrem por versão com problema pontual]].

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/movimentos-entrada-de-documento-simples|Movimentos Entrada de Documento Simples]]
- [[rotinas/_compartilhadas/movimentos-liquidacao-em-lote|Movimentos Liquidação]] (Individual/Em Lote/Cheques Pré Recebidos)

Observação: existe também **Movimentos Prorrogação Em Lote**, pré-mapeada apenas no Receber — é uma tela separada, que permite alterar vários documentos ao mesmo tempo (ainda não entrevistada).
