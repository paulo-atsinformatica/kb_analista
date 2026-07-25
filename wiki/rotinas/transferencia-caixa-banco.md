---
id: ROT-transferencia-caixa-banco
title: "Transferência de Caixa para Conta Bancária"
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
  - from: Transferência de Caixa para Conta Bancária
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
---

> [!NOTE] Correção de módulo
> Pré-mapeada originalmente também em `windows/bancos`. Confirmado com o analista que essa rotina existe apenas em `windows/caixa` e `windows/business`.

## Visão Geral
Rotina utilizada para transferir os valores das contas caixa para o banco.

## Quem Usa
Setor Administrativo/Financeiro.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Transferência de Conta Caixa para Conta Bancária**.

## Campos e Parâmetros Importantes
Rotina pouco utilizada, com poucos erros conhecidos.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
