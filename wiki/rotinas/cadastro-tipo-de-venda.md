---
id: ROT-cadastro-tipo-de-venda
title: "Cadastro de Tipo de Venda"
type: rotina
audience: all
modulos: ["windows/faturamento"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Cadastro de Tipo de Venda
    type: RELACIONA_COM
    to: NFE Digitação/Emissão de NFE
  - from: Cadastro de Tipo de Venda
    type: RELACIONA_COM
    to: Movimentos Pré-venda
  - from: Cadastro de Tipo de Venda
    type: RELACIONA_COM
    to: Movimentos Orçamentos
  - from: Cadastro de Tipo de Venda
    type: RELACIONA_COM
    to: Movimentos PDV
---

## Visão Geral
Processo utilizado para parametrizar e cadastrar as modalidades de venda que a empresa utiliza no sistema, definindo regras comerciais e financeiras.

## Quem Usa
Setor de Vendas.

## Módulos onde esta rotina existe
- windows/faturamento

## Como Usar (passo a passo)
Caminho: **Cadastros » Tipos de Venda » Tipos de Venda**.

Em Inclusão, informar a Descrição e selecionar os campos com as especificações desejadas para quando o tipo de venda for usado (Desconto/Acréscimo %, Comissão, Venda a Vista, Desconto Progressivo, regra de preço a usar — Preço 1-4/Custo/Médio/Calculado/Nenhum, além da aba Prazos).

## Campos e Parâmetros Importantes
O cadastro em si é simples, mas é importante entender que **tudo que envolve a venda é definido pelo Tipo de Venda selecionado**: o preço praticado, se há acréscimo ou desconto, e quais formas de pagamento podem ser usadas.

## Erros Comuns / Pontos de Atenção
Rotina simples, sem erros comuns registrados.

## Rotinas Relacionadas
Usado nas rotinas de venda:
- [[rotinas/nfe-digitacaoemissao-de-nfe|NFE Digitação/Emissão de NFE]]
- [[rotinas/movimentos-pre-venda|Movimentos Pré-venda]]
- [[rotinas/movimentos-orcamentos|Movimentos Orçamentos]]
- [[rotinas/movimentos-pdv|Movimentos PDV]]
