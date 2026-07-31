---
id: ROT-movimentos-liquidacao-individual
title: "Movimentos Liquidação Individual"
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
  - from: Movimentos Liquidação Individual
    type: RELACIONA_COM
    to: Movimentos Estorno
  - from: Movimentos Liquidação Individual
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
  - from: Movimentos Liquidação Individual
    type: RELACIONA_COM
    to: Movimentos Liquidação Impressão de Recibos
---

## Visão Geral
Faz a liquidação de documentos a pagar de forma **individual** (um documento por vez).

> [!NOTE] Comportamento diferente por módulo
> A mesma rotina, quando acessada pelo módulo **Contas a Receber**, liquida um documento **a receber** em vez de a pagar — o restante do funcionamento é equivalente.

## Quem Usa
Setor Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/contas-a-receber
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Liquidação » Individual** (atalho Ctrl+F3), ou pelo ícone "Liquidação" na barra de ferramentas.
2. Informar o Tipo de Operação e o Fornecedor.
3. Consultar o documento pelo número, ou clicar na lupa (F12) para buscar.
4. Informar o valor a ser pago, a Data do Pagamento, a Conta Caixa e demais informações necessárias (Forma de Pagamento, Banco/Agência/Conta se aplicável).
5. Confirmar com OK.

## Campos e Parâmetros Importantes
Sem dúvidas — rotina simples de utilizar.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/movimentos-estorno|Movimentos Estorno]] — liquidações feitas por esta rotina **podem** ser estornadas pela rotina genérica de Estorno (diferente da Liquidação Em Lote, que exige seu próprio botão de estorno).
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- Movimentos Liquidação Impressão de Recibos
