---
id: ROT-movimentos-emissao-de-nf-de-varios-pedidos
title: "Movimentos Emissão de NF de Vários Pedidos"
type: rotina
audience: all
modulos: ["windows/faturamento"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Movimentos Emissão de NF de Vários Pedidos
    type: RELACIONA_COM
    to: Cadastro de Tipos de Operação
  - from: Movimentos Emissão de NF de Vários Pedidos
    type: RELACIONA_COM
    to: Cadastro de Clientes
  - from: Movimentos Emissão de NF de Vários Pedidos
    type: RELACIONA_COM
    to: Movimentos Pré-venda
  - from: Movimentos Emissão de NF de Vários Pedidos
    type: RELACIONA_COM
    to: Movimentos PDV
  - from: Movimentos Emissão de NF de Vários Pedidos
    type: RELACIONA_COM
    to: Ordem de Serviço
---

> [!INFO] Nome exibido ao usuário
> Também conhecida no levantamento original como "NF de vários pedidos". Na tela do sistema aparece como **"NF de Vários Pedidos"**.

## Visão Geral
Rotina para emissão de Notas Fiscais de produtos e serviços, mais compacta que a Digitação/Emissão de NF-e. É usada quando um cliente fez diversas compras em pedidos diferentes e se quer emitir uma única nota reunindo todos esses pedidos.

## Quem Usa
Por ser rotina de emissão de notas: Financeiro, Fiscal, Vendas, etc.

## Módulos onde esta rotina existe
- windows/faturamento

## Como Usar (passo a passo)
Caminho: **Movimentos » Faturamento » Vendas » Notas Fiscais de Vários Pedidos**.

1. Informe o **Tipo de Operação** e o **Cliente**.
2. Escolha o **Tipo de pedido** a buscar: **Pedidos** (Pré-Venda, O.S., PDV) ou **Fiscal** (Cupom Fiscal, NFC-e, SAT, MF-e).
3. É possível filtrar os pedidos por período.
4. Marque um ou vários pedidos na lista (opção de marcar todos).
5. Encerre a seleção.
6. Informe as formas de pagamento, transportadora (se houver) e observações da nota.
7. Emita a nota (Faturar).

> [!WARNING]
> A rotina só emite NF de pedidos que já deram baixa no estoque.

## Campos e Parâmetros Importantes
Rotina pouco usada fora do contexto de vários pedidos — quem usa já conhece o fluxo e não costuma errar nos campos.

## Erros Comuns / Pontos de Atenção
- **Pedido não aparece na lista**: costuma ocorrer quando o pedido já foi iniciado na rotina de [[rotinas/nfe-digitacaoemissao-de-nfe|Digitação/Emissão de NF-e]] mas não foi concluído (ficou salvo em digitação). Nesse caso o pedido não fica disponível para seleção aqui. Solução: excluir a digitação pendente e retomar a rotina de NF de Vários Pedidos.

## Rotinas Relacionadas
- [[rotinas/cadastro-tipos-de-operacao|Cadastro de Tipos de Operação]] — exigido para emissão da nota.
- Cadastro de Clientes — exigido para emissão da nota.
- [[rotinas/movimentos-pre-venda|Movimentos Pré-venda]], [[rotinas/movimentos-pdv|Movimentos PDV]] e Ordem de Serviço — os pedidos exibidos para seleção vêm dessas rotinas.
