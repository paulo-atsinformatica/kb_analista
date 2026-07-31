---
id: ROT-movimentos-liquidacao-impressao-de-recibos
title: "Movimentos Liquidação Impressão de Recibos"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Movimentos Liquidação Impressão de Recibos
    type: RELACIONA_COM
    to: Movimentos Liquidação Individual
  - from: Movimentos Liquidação Impressão de Recibos
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Imprime o recibo de um documento a pagar — pode ser feito mesmo para documentos ainda não liquidados. Também permite reimprimir recibos já emitidos.

## Quem Usa
Rotina pouco utilizada, pelo setor Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Movimentos » Liquidação » Impressão de Recibos**.
2. Filtrar por Empresa, Fornecedor, Data de Vencimento (com opção "Incluir documentos não liquidados").
3. Selecionar os documentos desejados.
4. Solicitar a impressão.

## Campos e Parâmetros Importantes
Sem dúvidas — rotina simples de utilizar.

## Erros Comuns / Pontos de Atenção
Sem erros conhecidos, além da ressalva geral: ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- Movimentos Liquidação Individual
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
