---
id: ROT-movimentos-cruzamento-de-contas
title: "Movimentos Cruzamento de Contas"
type: rotina
audience: a-definir
modulos: ["windows/contas-a-pagar"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Movimentos Cruzamento de Contas
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Faz o abatimento entre valor a pagar e valor a receber, quando o fornecedor também é cliente. Confirma a importância de ter os cadastros de fornecedor e cliente associados (ver [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]).

## Quem Usa
Setor do Financeiro responsável por contas a pagar e receber.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Movimentos » Cruzamento de Contas**.

## Campos e Parâmetros Importantes
Rotina simples, mas costuma gerar dúvida no preenchimento dos valores. Regra importante: o **valor a pagar nunca pode ser maior que o valor a receber**, e vice-versa.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- Documentos a receber dos clientes (Contas a Receber)
