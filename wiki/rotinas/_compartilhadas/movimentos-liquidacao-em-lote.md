---
id: ROT-movimentos-liquidacao-em-lote
title: "Movimentos Liquidação Em Lote"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/contas-a-receber", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Movimentos Liquidação Em Lote
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
  - from: Movimentos Liquidação Em Lote
    type: RELACIONA_COM
    to: Movimentos Entrada de Documento Simples
---

## Visão Geral
Faz a liquidação de documentos a pagar em lote — ou seja, mais de um documento ao mesmo tempo. Pode ser filtrada por fornecedor ou pesquisada sem filtro.

> [!NOTE] Comportamento diferente por módulo
> A mesma rotina, quando acessada pelo módulo **Contas a Receber**, liquida documentos **a receber** em vez de a pagar — o restante do funcionamento é equivalente.

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/contas-a-receber
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Liquidação » Em Lote** (atalho ao lado de Individual, Com Cheques Pré-Recebidos e Impressão de Recibos).
2. Filtrar pelo fornecedor (opcional), ou pesquisar sem filtro.
3. Selecionar os documentos que serão liquidados (os não selecionados permanecem em aberto).
4. Informar a Conta Caixa e a Forma de Pagamento.
5. Confirmar a liquidação.

Essa é a única rotina de liquidação em lote que permite a forma de pagamento **aproveitamento de crédito** (as demais rotinas de liquidação não suportam essa forma).

## Campos e Parâmetros Importantes
- O botão de engrenagem (**Configurar**) — ver [[procedimentos/configuracao-restrita-mestre-admin|acesso restrito a MESTRE/ADMIN]] — abre a tela "Configura Liq. em Lote do Pagar", onde se define: ao liquidar vários documentos, se o sistema gera **apenas um lançamento**, **um lançamento para cada documento**, ou **pergunta ao usuário**; e se mantém a observação e/ou a conta caixa do documento original.

## Erros Comuns / Pontos de Atenção
- Se a liquidação foi feita por esta rotina, o **estorno também deve ser feito por ela mesma** (botão específico na tela) — não pela rotina genérica de Movimentos Estorno, que só funciona para liquidações feitas via Liquidação Individual.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- [[rotinas/_compartilhadas/movimentos-entrada-de-documento-simples|Movimentos Entrada de Documento Simples]]
