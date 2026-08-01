---
id: ROT-relatorios-contas-a-pagar-saldo
title: "Relatórios Contas a Pagar Saldo"
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
  - from: Relatórios Contas a Pagar Saldo
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Relatório utilizado apenas para mostrar o valor dos documentos a pagar do fornecedor que estão em aberto.

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Relatórios » Contas a Pagar » Saldos**.
2. Informar o Fornecedor.
3. Informar o Tipo de Documento, Tipo de Fornecedor e/ou Período desejados (opcional).
4. Clicar em **Imprimir** — o relatório mostra apenas o valor em aberto para pagar (Vencidos, A Vencer e Total).

Rotina simples.

## Campos e Parâmetros Importantes
Rotina simples, sem pontos de atenção relevantes segundo o analista.

## Erros Comuns / Pontos de Atenção
Sem erros comuns — [[procedimentos/erros-apenas-por-versao-com-problema|problemas só ocorrem por versão com problema pontual]].

## Rotinas Relacionadas
- Documentos a pagar
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- Demais rotinas relacionadas a documentos a pagar
