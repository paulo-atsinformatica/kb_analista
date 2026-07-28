---
id: ROT-consultas-grafico-posicao-contas-a-pagar
title: "Consultas Gráfico Posição Contas a Pagar"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Consultas Gráfico Posição Contas a Pagar
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Analítica
  - from: Consultas Gráfico Posição Contas a Pagar
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Sintética
  - from: Consultas Gráfico Posição Contas a Pagar
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Saldos
  - from: Consultas Gráfico Posição Contas a Pagar
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
---

## Visão Geral
Gera um gráfico (pizza) mostrando a posição dos títulos em aberto — por valor ou por quantidade de títulos — separando Atrasados x Em Dia. Pode ser filtrado por conta caixa.

## Quem Usa
Financeiro, parte do contas a pagar.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/business

## Como Usar (passo a passo)
1. Acessar **Consultas » Gráfico Posição Contas a Pagar**.
2. Opcionalmente, filtrar por Conta Caixa.
3. Escolher a opção: Considerando Valor, ou Considerando Quantidade de Títulos.

## Campos e Parâmetros Importantes
Sem dúvidas — rotina tranquila.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- Consultas Contas a Pagar Analítica
- Consultas Contas a Pagar Sintética
- Consultas Contas a Pagar Saldos
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
