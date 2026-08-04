---
id: ROT-relatorios-contas-a-pagar-cheques
title: "Relatórios Contas a Pagar / Cheques"
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
  - from: Relatórios Contas a Pagar / Cheques
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Relatório usado para filtrar os documentos a pagar que foram gerados com o tipo de documento **cheque**.

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Relatórios » Contas a Pagar » Contas a Pagar / Cheques**.
2. Informar o Fornecedor.
3. Informar o Período de Vencimento e/ou Data de Emissão desejados.
4. Clicar em **Imprimir**.

Rotina simples, sem muitos filtros disponíveis.

## Campos e Parâmetros Importantes
Basta informar o fornecedor e as datas de acordo com o que se deseja gerar — sem outros pontos de atenção.

## Erros Comuns / Pontos de Atenção
Atenção ao período de datas informado, pois influencia diretamente o resultado do relatório.

## Rotinas Relacionadas
- Documentos a pagar
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- Cheques lançados
