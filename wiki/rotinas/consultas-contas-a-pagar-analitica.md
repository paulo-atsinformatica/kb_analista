---
id: ROT-consultas-contas-a-pagar-analitica
title: "Consultas Contas a Pagar Analítica"
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
  - from: Consultas Contas a Pagar Analítica
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Sintética
  - from: Consultas Contas a Pagar Analítica
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Saldos
  - from: Consultas Contas a Pagar Analítica
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Consulta os documentos em aberto a pagar, por fornecedor e período. Por ser a versão Analítica, traz informações mais completas: tipo de documento, código do documento, histórico.

## Quem Usa
Setor Financeiro, voltado para movimentações a pagar.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/business

## Como Usar (passo a passo)
1. Acessar **Consultas » Contas a Pagar » Analítica** (atalho Ctrl+A), ou pelo ícone na barra de ferramentas.

## Campos e Parâmetros Importantes
Sem dúvidas — rotina simples de utilizar.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- Consultas Contas a Pagar Sintética
- Consultas Contas a Pagar Saldos
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
