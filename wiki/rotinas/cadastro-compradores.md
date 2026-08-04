---
id: ROT-cadastro-compradores
title: "Cadastro de Compradores"
type: rotina
audience: all
modulos: ["windows/compras", "windows/faturamento"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Cadastro de Compradores
    type: RELACIONA_COM
    to: Movimentos Cotação de Preços Abertura de Cotações
  - from: Cadastro de Compradores
    type: RELACIONA_COM
    to: Movimentos Solicitação de Compras de Produtos
---

## Visão Geral
Cadastro interno para informar o comprador. É utilizado para solicitar orçamento de fornecedores.

## Quem Usa
Setor de Compras.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/compras — usado especificamente nas rotinas relacionadas a compras (cotação e solicitação de compra)

## Como Usar (passo a passo)
Caminho: **Cadastros » Compradores**.

Tela simples: preencher Código, Nome, E-Mail e Limite Sem Autorização, e salvar (Inclusão).

## Campos e Parâmetros Importantes
Nenhum ponto de atenção específico.

## Erros Comuns / Pontos de Atenção
Rotina simples, sem erros comuns registrados.

## Rotinas Relacionadas
- [[rotinas/movimentos-cotacao-de-precos-abertura-de-cotacoes|Movimentos Cotação de Preços - Abertura de Cotações]]
- [[rotinas/movimentos-solicitacao-de-compras-de-produtos|Movimentos Solicitação de Compras de Produtos]]

Não tem relação com o campo de comprador na Ordem de Compra / Entrada de Produtos, apesar de existir ordem de compra nessa rotina.
