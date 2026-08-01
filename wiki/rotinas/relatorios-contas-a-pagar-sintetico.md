---
id: ROT-relatorios-contas-a-pagar-sintetico
title: "Relatórios Contas a Pagar Sintético"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Relatórios Contas a Pagar Sintético
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Mesma finalidade do [[rotinas/_compartilhadas/relatorios-contas-a-pagar-analitico|Relatórios Contas a Pagar Analítico]], mas mais simples, com menos filtros e trazendo informações menos completas (resumo por data de emissão/vencimento, com totais de Vencidos e A Vencer).

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Relatórios » Contas a Pagar » Sintético** (atalho **Ctrl+T**).
2. Informar o Período de Emissão/Vencimento desejado.
3. Opcionalmente, marcar um ou mais fornecedores na lista (ou marcar **Todos** para trazer todos os documentos em aberto).
4. Clicar em **Imprimir**.

## Campos e Parâmetros Importantes
Marcar o checkbox **"Todos"** apenas quando quiser trazer os documentos em aberto de todos os fornecedores — caso contrário, rotina simples.

## Erros Comuns / Pontos de Atenção
Sem erros comuns — [[procedimentos/erros-apenas-por-versao-com-problema|problemas só ocorrem por versão com problema pontual]].

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- Documentos a pagar
