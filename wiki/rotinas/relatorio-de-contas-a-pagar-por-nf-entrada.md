---
id: ROT-relatorio-de-contas-a-pagar-por-nf-entrada
title: "Relatório de Contas a Pagar Por NF Entrada"
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
  - from: Relatório de Contas a Pagar Por NF Entrada
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Rotina de relatório que gera os documentos a pagar somente das entradas de notas fiscais, mostrando as informações da nota (fornecedor, número da nota, data de entrada, vencimento, parcelas e valores).

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Relatórios » Relatório de Contas a Pagar Por NF Entrada**.
2. Informar o Fornecedor.
3. Informar o período de Entrada e/ou Vencimento desejado.
4. Clicar em **Imprimir**.

## Campos e Parâmetros Importantes
Rotina simples, sem pontos de atenção relevantes segundo o analista.

## Erros Comuns / Pontos de Atenção
Sem erros comuns — [[procedimentos/erros-apenas-por-versao-com-problema|problemas só ocorrem por versão com problema pontual]].

## Rotinas Relacionadas
- É associada à entrada de produtos (nota fiscal de entrada) e ao [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]] — não tem relação com Movimentos Entrada de Documento Simples.
