---
id: ROT-cadastro-tipos-de-operacao
title: "Cadastro de Tipos de Operação"
type: rotina
audience: all
modulos: ["windows/faturamento", "windows/livros-fiscais"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Cadastro de Tipos de Operação
    type: RELACIONA_COM
    to: NFE Digitação/Emissão de NFE
  - from: Cadastro de Tipos de Operação
    type: RELACIONA_COM
    to: Movimentos Emissão de NF de Vários Pedidos
  - from: Cadastro de Tipos de Operação
    type: RELACIONA_COM
    to: Movimentos Entrada de Produtos
  - from: Cadastro de Tipos de Operação
    type: RELACIONA_COM
    to: Movimentos Entrada de Documento Simples
  - from: Cadastro de Tipos de Operação
    type: RELACIONA_COM
    to: Movimentos Liquidação Individual
  - from: Cadastro de Tipos de Operação
    type: RELACIONA_COM
    to: Movimentos Liquidação Em Lote
---

## Visão Geral
Cadastro da operação (tipo de movimento) que será utilizada na emissão de notas fiscais. Nela se define o CFOP e um conjunto de comportamentos: se gera financeiro (contas a pagar/receber), se atualiza estoque, se considera em relatórios de vendas, etc.

## Quem Usa
Quem for emitir uma nota fiscal — geralmente perfil Fiscal, Financeiro ou Contábil.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/livros-fiscais — usada na consulta/relatório de Notas Fiscais Emitidas

## Como Usar (passo a passo)
Caminho: **Cadastros » Tipos de Operação**.

1. Clique em **Inclusão**.
2. Informe a **Descrição** — serve para identificar a situação de uso da operação (ex: "Venda de Mercadoria para fora do estado").
3. Selecione o **Tipo de Operação**: existem 8 opções numéricas (1 a 8 — Serviço, Venda, Revenda, Revenda/Serviço, Entradas Pagar, Liquidação a Pagar, Liquidação a Receber, Entradas Receber) e 5 opções alfabéticas (A a E — Ent. Via Doc. Próprio, Outras Saídas, Nota de Compl. de Saída, Nota de Compl. de Entr., CT-e).
4. Informe o **CFOP** da operação — é possível informar até 4 CFOPs na mesma operação.
5. Navegue pelas subabas conforme a necessidade:
   - **Complementos**: se atualiza estoque, considera comissão, considera em vendas, etc.
   - **ICMS/ST/IPI**: situações tributárias específicas.
   - **Integração**: se gera financeiro, e se integra com Caixa, Bancos ou Pré-datados.
   - Demais abas (NF-e, PIS/COFINS, SPED) com dados específicos.

## Campos e Parâmetros Importantes
- **CFOP**: embora seja possível informar até 4 CFOPs na mesma operação, **não se pode misturar CFOPs tributados com CFOPs de Substituição Tributária (ST)** na mesma operação.

## Erros Comuns / Pontos de Atenção
Rotina simples, com poucos erros no uso. Ponto de atenção: **evitar alterar uma operação já em uso**, pois nem toda alteração fica registrada em histórico. Se for necessária uma configuração diferente para uma situação específica, o recomendado é **criar uma nova operação semelhante** em vez de alterar a existente.

## Rotinas Relacionadas
O Tipo de Operação cadastrado aqui é utilizado nas rotinas de emissão de nota:
- [[rotinas/_compartilhadas/nfe-digitacaoemissao-de-nfe|NFE Digitação/Emissão de NFE]]
- [[rotinas/movimentos-emissao-de-nf-de-varios-pedidos|Movimentos Emissão de NF de Vários Pedidos]]

E também nas rotinas de entrada e liquidação de documentos (tanto Contas a Pagar quanto Contas a Receber):
- [[rotinas/movimentos-entrada-de-produtos|Movimentos Entrada de Produtos]] (entrada de notas de compra)
- [[rotinas/_compartilhadas/movimentos-entrada-de-documento-simples|Movimentos Entrada de Documento Simples]] (entrada de documentos a pagar/receber)
- [[rotinas/_compartilhadas/movimentos-liquidacao-individual|Movimentos Liquidação Individual]] e [[rotinas/_compartilhadas/movimentos-liquidacao-em-lote|Movimentos Liquidação Em Lote]] (liquidação de contas a pagar/receber)
