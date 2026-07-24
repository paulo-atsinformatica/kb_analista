---
id: ROT-relatorios-fechamento-de-caixa
title: "Relatórios Fechamento de Caixa"
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
  - from: Relatórios Fechamento de Caixa
    type: RELACIONA_COM
    to: Fechamento de Caixa
  - from: Relatórios Fechamento de Caixa
    type: RELACIONA_COM
    to: Cadastro de Operadores de Caixa
  - from: Relatórios Fechamento de Caixa
    type: RELACIONA_COM
    to: Cadastro de Turnos
---

## Visão Geral
Relatório que mostra os caixas que foram **fechados**, junto com os valores. Pode ser filtrado por filial, período, operador, e tipo de relatório (Analítico ou Sintético).

## Quem Usa
Setor administrativo da empresa, ou responsável pelos caixas.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Fechamento de Caixa**.

## Campos e Parâmetros Importantes
Sem dúvidas — rotina tranquila de gerar.

## Erros Comuns / Pontos de Atenção
Sem erros. Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/fechamento-de-caixa|Fechamento de Caixa]]
- [[rotinas/cadastro-operadores|Cadastro de Operadores de Caixa]]
- [[rotinas/_compartilhadas/cadastro-turnos|Cadastro de Turnos]]
