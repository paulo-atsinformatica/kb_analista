---
id: ROT-movimentos-estorno
title: "Movimentos Estorno"
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
  - from: Movimentos Estorno
    type: RELACIONA_COM
    to: Movimentos Liquidação Individual
  - from: Movimentos Estorno
    type: RELACIONA_COM
    to: Movimentos Liquidação Em Lote
  - from: Movimentos Estorno
    type: RELACIONA_COM
    to: Movimentos Liquidação com Cheques Pré Recebidos
---

## Visão Geral
Estorna um documento (a pagar ou a receber, dependendo do módulo) que foi liquidado pela rotina de **Liquidação Individual**. Se o documento foi liquidado por outra rotina (Em Lote, ou com Cheques Pré-Datados), não pode ser estornado por aqui — essas rotinas têm seu próprio estorno embutido.

## Quem Usa
Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/contas-a-receber
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Estorno** (atalho Ctrl+F4), ou pelo ícone "Estornos" na barra de ferramentas.
2. Informar o Fornecedor (e opcionalmente Período ou Nº do Documento).
3. Clicar em Localizar/Buscar para listar os documentos liquidados pela rotina de Liquidação Individual.
4. Dar duplo clique no documento desejado e confirmar o estorno.

## Campos e Parâmetros Importantes
- Após o estorno, o documento volta a ficar **em aberto** para ser liquidado novamente.

## Erros Comuns / Pontos de Atenção
- Se o documento foi liquidado por **outra rotina** (Em Lote, Cheques Pré-Datados) e você tentar estornar por aqui, o documento **nunca será encontrado**.

## Rotinas Relacionadas
- Movimentos Liquidação Individual
- Movimentos Liquidação Em Lote
- Movimentos Liquidação com Cheques Pré Recebidos
