---
id: ROT-cadastro-moedas-cotacoes
title: "Cadastro de Moedas (Cotações)"
type: rotina
audience: all
modulos: ["windows/contas-a-receber", "windows/contas-a-pagar", "windows/bancos", "windows/faturamento", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Cadastro de Moedas (Cotações)
    type: RELACIONA_COM
    to: Cadastro de Moedas (Identificação)
---

## Visão Geral
Cadastra as cotações das moedas já cadastradas no sistema (via Cadastro de Moedas - Identificação).

## Quem Usa
Rotina pouco utilizada, mas pelo setor Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-receber
- windows/contas-a-pagar
- windows/bancos
- windows/faturamento
- windows/business

## Como Usar (passo a passo)
1. Acessar **Cadastros » Moedas » Cadastro de Valores de Moedas**.
2. Informar a Moeda, a Data Cotação e o Valor.

## Campos e Parâmetros Importantes
- Não é possível informar cotação para a moeda **01 (REAL)**, que é a moeda padrão do sistema.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- Cadastro de Moedas (Identificação) — define as moedas que podem ter cotação cadastrada aqui.
