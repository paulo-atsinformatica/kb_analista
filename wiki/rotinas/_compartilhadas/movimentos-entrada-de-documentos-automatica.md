---
id: ROT-movimentos-entrada-de-documentos-automatica
title: "Movimentos Entrada de Documentos Automática"
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
  - from: Movimentos Entrada de Documentos Automática
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
  - from: Movimentos Entrada de Documentos Automática
    type: RELACIONA_COM
    to: Cadastro Histórico Padrão
  - from: Movimentos Entrada de Documentos Automática
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
  - from: Movimentos Entrada de Documentos Automática
    type: RELACIONA_COM
    to: Movimentos Entrada de Documento Simples
---

## Visão Geral
Gera documentos recorrentes para vários meses de uma vez — por exemplo, uma conta fixa mensal (internet, telefone) com o mesmo valor e fornecedor.

> [!NOTE] Comportamento diferente por módulo
> A mesma rotina, quando acessada pelo módulo **Contas a Receber**, gera documentos **a receber** em vez de a pagar — o restante do funcionamento é equivalente.

## Quem Usa
Setor Financeiro, voltado para contas a pagar.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/contas-a-receber
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Entrada de Documentos » Automática**.
2. Informar Tipo de Operação, Filial, Fornecedor, Tipo de Documento, Nº Documento, Emissão, Dia de Vencimento e Mês/Ano Inicial.
3. Informar Histórico, Conta Caixa, Moeda, Valor da Parcela, Desconto da Parcela, Nº de Parcelas e Centro de Custo.
4. Opcionalmente, clicar em **Alterar Parcelas** para customizar vencimento/valor de cada parcela individualmente.
5. Confirmar em OK — o sistema gera todos os documentos das parcelas de uma vez.

## Campos e Parâmetros Importantes
- **Gravar como data de competência dos documentos a data de vencimento**: grava a data de competência no lugar da data informada (data em que o documento foi feito).
- **Repetir conta crédito e débito para todas as parcelas**: repete a mesma conta crédito/débito em todas as parcelas lançadas.

## Erros Comuns / Pontos de Atenção
- Informar o **dia de vencimento** ou a **quantidade de parcelas** incorretos.
- Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão, fora isso.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- [[rotinas/_compartilhadas/cadastro-historico-padrao|Cadastro Histórico Padrão]]
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
- [[rotinas/_compartilhadas/movimentos-entrada-de-documento-simples|Movimentos Entrada de Documento Simples]]
