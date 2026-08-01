---
id: ROT-relatorios-contas-a-pagar-analitico
title: "Relatórios Contas a Pagar Analítico"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/contas-a-receber", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Relatórios Contas a Pagar Analítico
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Relatório mais completo para gerar os documentos a pagar dos fornecedores. Se nenhum filtro for informado, traz todas as informações em aberto para pagar.

> [!NOTE] Comportamento diferente por módulo
> No módulo **Contas a Receber**, a rotina equivalente pré-mapeada como "Relatórios Analítico de Vencimentos" mostra os documentos **a receber** dos clientes, ao invés de a pagar dos fornecedores (os filtros passam a ser sobre o cliente, não sobre o fornecedor).

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/contas-a-receber
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Contas a Pagar » Analítico** (atalho **Ctrl+L**, ou ícone "Contas a Pagar" no menu).
2. Informar os filtros desejados (Filtro de Tipos de Documentos, Tipo de Fornecedor, Conta Caixa, Centro de Custo, Período de Emissão/Vencimento, Fornecedor, Moeda).
3. Escolher o tipo de Relatório (Simples/Completo/Completo por Data/Completo c/ Centro Custo/Somente Resumo Mensal) e a Ordem (Data/Alfabética).
4. Clicar em **Imprimir** ou **Exportar**.

## Campos e Parâmetros Importantes
Para filtrar por um fornecedor específico, é necessário marcar a opção **"Escolher fornecedor"** — isso habilita o campo para informar qual fornecedor deve ser filtrado.

## Erros Comuns / Pontos de Atenção
Sem informar nenhum filtro, o relatório traz todas as informações em aberto para pagar — atenção ao volume de dados gerado nesse caso.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- Documentos a pagar
- Contas Caixa
- Centro de Custo
