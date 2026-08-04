---
id: ROT-relatorios-contas-pagas
title: "Relatório de Contas Pagas"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Relatório de Contas Pagas
    type: RELACIONA_COM
    to: Movimentos Liquidação Em Lote
  - from: Relatório de Contas Pagas
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Rotina usada para gerar o relatório com os documentos a pagar que já foram pagos (liquidados).

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Contas a Pagar » Contas Pagas** (atalho **Ctrl+G**, ou ícone "Contas Pagas" no menu).
2. Informar os filtros desejados (Fornecedor, Tipo de Documento, Tipo de Fornecedor, Moeda, Forma Pagamento, Banco, Conta Caixa, Centro Custo, período de Pagos/Emitidos/Vencidos, etc.) — é uma rotina de relatório, então todas as informações geradas dependem dos filtros informados.
3. Escolher as opções de Visualizar (Históricos, Observações, Contas Caixa), Totalização, Ordenar por Data e Tipo de Relatório (Analítico/Sintético/Resumido).
4. Clicar em **Imprimir** ou **Exportar**.

## Campos e Parâmetros Importantes
Por ser uma rotina de filtros, não há um campo específico que gere confusão — o uso varia conforme a necessidade de cada cliente ao gerar o relatório.

## Erros Comuns / Pontos de Atenção
Sem erros comuns — [[procedimentos/erros-apenas-por-versao-com-problema|problemas só ocorrem por versão com problema pontual]].

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/movimentos-liquidacao-em-lote|Movimentos Liquidação]] (documentos liquidados)
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
