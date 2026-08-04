---
id: ROT-clientes-classificacao
title: "Classificação de Clientes"
type: rotina
audience: all
modulos: ["windows/faturamento", "windows/contas-a-receber"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Classificação de Clientes
    type: RELACIONA_COM
    to: Cadastro de Clientes
---

## Visão Geral
Cadastro para diferenciação/classificação de clientes. Existe um campo próprio no Cadastro de Clientes, chamado **Status**, que usa essa classificação.

## Quem Usa
Rotina pouco usada. Geralmente Gestores e setor de Vendas.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/contas-a-receber

## Como Usar (passo a passo)
Caminho: **Cadastros » Clientes » Classificação de Clientes**.

Em Inclusão, informar a Descrição e salvar. O valor cadastrado fica disponível no campo **Status**, na aba Complementares do [[rotinas/cadastro-clientes|Cadastro de Clientes]].

## Campos e Parâmetros Importantes
Rotina muito simples (Código, Descrição), sem pontos de atenção.

## Erros Comuns / Pontos de Atenção
Nenhum erro comum registrado.

## Rotinas Relacionadas
- [[rotinas/cadastro-clientes|Cadastro de Clientes]] — usada no campo Status. Não se relaciona com nenhuma outra rotina.
