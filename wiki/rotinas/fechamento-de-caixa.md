---
id: ROT-fechamento-de-caixa
title: "Fechamento de Caixa"
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
  - from: Fechamento de Caixa
    type: RELACIONA_COM
    to: Abertura de Caixa
  - from: Fechamento de Caixa
    type: RELACIONA_COM
    to: Cadastro de Turnos
  - from: Fechamento de Caixa
    type: RELACIONA_COM
    to: Cadastro de Operadores de Caixa
  - from: Fechamento de Caixa
    type: RELACIONA_COM
    to: Consultas Livro Caixa
---

## Visão Geral
Rotina usada para fazer a conferência do caixa do dia e realizar o fechamento.

## Quem Usa
Operador do caixa, ou responsável pelo fechamento dos caixas.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Fechamento de Caixa**.
2. Informar o Usuário que abriu o caixa, o Turno aberto, e a Data/Hora do fechamento.

## Campos e Parâmetros Importantes
- Existe um campo que permite reabrir o caixa depois de fechado, caso necessário. Ele já vem **habilitado por padrão** — o cuidado é não desmarcá-lo sem necessidade.

## Erros Comuns / Pontos de Atenção
- Informar **data e hora incorretas** no fechamento é o erro mais comum — exige atenção.

## Rotinas Relacionadas
- [[rotinas/abertura-de-caixa|Abertura de Caixa]] — o fechamento deve usar o mesmo turno da abertura.
- [[rotinas/_compartilhadas/cadastro-turnos|Cadastro de Turnos]]
- [[rotinas/cadastro-operadores|Cadastro de Operadores de Caixa]]
- [[rotinas/consultas-livro-caixa|Consultas Livro Caixa]]
