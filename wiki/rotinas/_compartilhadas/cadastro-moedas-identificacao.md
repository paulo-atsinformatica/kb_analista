---
id: ROT-cadastro-moedas-identificacao
title: "Cadastro de Moedas (Identificação)"
type: rotina
audience: all
modulos: ["windows/contas-a-receber", "windows/contas-a-pagar", "windows/bancos", "windows/business", "windows/faturamento"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Cadastro de Moedas (Identificação)
    type: RELACIONA_COM
    to: Cadastro de Moedas (Cotações)
  - from: Cadastro de Moedas (Identificação)
    type: RELACIONA_COM
    to: Consultas Contas Pagas
  - from: Cadastro de Moedas (Identificação)
    type: RELACIONA_COM
    to: Consultas Contas a Pagar no Mês
---

## Visão Geral
Cadastra as moedas do sistema. Por padrão, o sistema já traz cadastrado o **Real (R$)**.

## Quem Usa
Rotina pouco utilizada, pelo setor Financeiro/Administrativo.

## Módulos onde esta rotina existe
- windows/contas-a-receber
- windows/contas-a-pagar
- windows/bancos
- windows/business
- windows/faturamento

## Como Usar (passo a passo)
1. Acessar **Cadastros » Moedas » Cadastro de Moedas**.
2. Informar Código, Descrição, Símbolo, Máscara, e a Operação (Multiplica ou Divide).

## Campos e Parâmetros Importantes
- A opção **Operação** define se a conversão da moeda multiplica ou divide o valor pela cotação: se configurada para Multiplicar, o valor sempre será multiplicado; se Dividir, sempre será dividido.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-moedas-cotacoes|Cadastro de Moedas (Cotações)]]
- Consultas Contas Pagas, Consultas Contas a Pagar no Mês, e demais rotinas com campo Moeda.
