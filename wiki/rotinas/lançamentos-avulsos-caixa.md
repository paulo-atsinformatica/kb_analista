---
id: ROT-lançamentos-avulsos-caixa
title: "Lançamentos Avulsos de Caixa"
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
  - from: Lançamentos Avulsos de Caixa
    type: RELACIONA_COM
    to: Consultas Livro Caixa
  - from: Lançamentos Avulsos de Caixa
    type: RELACIONA_COM
    to: Consultas Saldo Geral
  - from: Lançamentos Avulsos de Caixa
    type: RELACIONA_COM
    to: Consultas Saldo das Contas
  - from: Lançamentos Avulsos de Caixa
    type: RELACIONA_COM
    to: Movimentos Fechamento de Caixa Financeiro
---

## Visão Geral
Permite fazer lançamentos avulsos no caixa — entradas e saídas — feitos diretamente através de contas caixa.

## Quem Usa
Operador do caixa, setor administrativo.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Lançamentos** (atalho Ctrl+F2).

## Campos e Parâmetros Importantes
- Para um lançamento de **saída**, a conta caixa deve ser **Débito**; para um lançamento de **entrada**, a conta caixa deve ser **Crédito** (mesma regra do Cadastro de Contas Caixa).

## Erros Comuns / Pontos de Atenção
- Atenção à **conta caixa informada** no lançamento, para que o movimento (entrada/saída) seja registrado corretamente.

## Rotinas Relacionadas
- [[rotinas/consultas-livro-caixa|Consultas Livro Caixa]] e demais rotinas que consultam as movimentações do caixa (Saldo Geral, Saldo das Contas).
- Movimentos Fechamento de Caixa Financeiro
