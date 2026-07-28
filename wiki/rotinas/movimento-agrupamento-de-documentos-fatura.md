---
id: ROT-movimento-agrupamento-de-documentos-fatura
title: "Movimento Agrupamento de Documentos (Fatura)"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Movimento Agrupamento de Documentos (Fatura)
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
  - from: Movimento Agrupamento de Documentos (Fatura)
    type: RELACIONA_COM
    to: Movimentos Entrada de Documento Simples
  - from: Movimento Agrupamento de Documentos (Fatura)
    type: RELACIONA_COM
    to: Movimentos Estorno
---

## Visão Geral
Agrupa documentos a pagar pendentes, criando um novo documento (tipo **FT** - Fatura) com uma nova data de vencimento. Serve tanto para criar um novo documento com nova data quanto para consolidar vários documentos em um só.

## Quem Usa
Setor Financeiro do contas a pagar.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Agrupamento de Documentos (Fatura)**.
2. Filtrar os documentos pelo fornecedor.
3. Selecionar quais documentos deseja agrupar (aba "Documentos a agrupar").
4. Na aba "Documentos a gerar", informar o novo Prazo de pagamento (ou parcelas manuais), Conta Caixa e Centro de Custo.
5. Clicar em **Gera Documento**.

## Campos e Parâmetros Importantes
- Após gerar, o sistema mostra o **número da fatura gerada** — importante anotar, pois facilita listar ou estornar esse agrupamento depois.
- O botão **Listar/Estornar** (na mesma tela) permite filtrar por Nº da fatura ou fornecedor, ver os documentos agrupados, e cancelar o agrupamento (os documentos voltam a ficar em aberto).

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- Movimentos Entrada de Documento Simples
- Movimentos Estorno
