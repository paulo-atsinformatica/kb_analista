---
id: ROT-cadastro-prazos-de-pagamento
title: "Cadastro de Prazos de Pagamento"
type: rotina
audience: all
modulos: ["windows/faturamento", "windows/contas-a-receber", "windows/contas-a-pagar"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Cadastro de Prazos de Pagamento
    type: RELACIONA_COM
    to: NFE Digitação/Emissão de NFE
  - from: Cadastro de Prazos de Pagamento
    type: RELACIONA_COM
    to: Movimentos Emissão de NF de Vários Pedidos
  - from: Cadastro de Prazos de Pagamento
    type: RELACIONA_COM
    to: Movimentos Pré-venda
  - from: Cadastro de Prazos de Pagamento
    type: RELACIONA_COM
    to: Movimentos Orçamentos
  - from: Cadastro de Prazos de Pagamento
    type: RELACIONA_COM
    to: Movimentos PDV
  - from: Cadastro de Prazos de Pagamento
    type: RELACIONA_COM
    to: Movimentos Entrada de Documento Simples
  - from: Cadastro de Prazos de Pagamento
    type: RELACIONA_COM
    to: Movimentos Liquidação Individual
---

## Visão Geral
Rotina utilizada para cadastrar os prazos de pagamento que serão utilizados no Contas a Receber (e também no Contas a Pagar).

## Quem Usa
Financeiro, Gestor, Vendas, etc.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/contas-a-receber
- windows/contas-a-pagar

## Como Usar (passo a passo)
Caminho: **Cadastros » Prazos de Pagamento**.

1. Informe a Descrição.
2. Selecione o tipo de condição: **Prazos** ou **Parcelas**.

## Campos e Parâmetros Importantes
Diferença entre as duas condições de pagamento:
- **Prazos**: até 12 prazos, cada um com um percentual e um intervalo de dias diferente entre si.
- **Parcelas**: define o número de parcelas (pode ser maior que 12), mas o intervalo de dias entre elas é fixo.

## Erros Comuns / Pontos de Atenção
Rotina simples. O único ponto de confusão comum é entre as opções **Prazos** e **Parcelas** (ver diferença acima).

## Rotinas Relacionadas
Usada em qualquer rotina que utilize prazo de pagamento:
- [[rotinas/nfe-digitacaoemissao-de-nfe|NFE Digitação/Emissão de NFE]]
- [[rotinas/movimentos-emissao-de-nf-de-varios-pedidos|Movimentos Emissão de NF de Vários Pedidos]]
- [[rotinas/movimentos-pre-venda|Movimentos Pré-venda]]
- [[rotinas/movimentos-orcamentos|Movimentos Orçamentos]]
- [[rotinas/movimentos-pdv|Movimentos PDV]]
- Ordem de Serviço (O.S.)
- [[rotinas/_compartilhadas/movimentos-entrada-de-documento-simples|Movimentos Entrada de Documento Simples]] (Contas a Pagar/Receber)
- [[rotinas/_compartilhadas/movimentos-liquidacao-individual|Movimentos Liquidação Individual]] (Contas a Pagar/Receber)
