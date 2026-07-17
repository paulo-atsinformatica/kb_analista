---
id: ROT-cadastro-contas-caixa
title: "Cadastro de Contas Caixa"
type: rotina
audience: all
modulos: ["windows/caixa", "windows/bancos", "windows/contas-a-receber", "windows/contas-a-pagar", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Cadastro de Contas Caixa
    type: RELACIONA_COM
    to: Relatórios Demonstração de Resultados (DRE)
---

## Visão Geral
Cadastro do plano de contas caixa, usado para os lançamentos do sistema. As contas são organizadas em hierarquia: primeiro se cadastram as contas **pai**, depois as contas **filhas** vinculadas a elas.

Exemplo de hierarquia:
- `01` → Despesas
- `01.01` → Despesas » Fornecedores
- `01.01.001` → Pagamento a Vista (para Fornecedores)

## Quem Usa
Setor Financeiro/Administrativo.

## Módulos onde esta rotina existe
- windows/caixa
- windows/bancos
- windows/contas-a-receber
- windows/contas-a-pagar
- windows/business

## Como Usar (passo a passo)
1. Acessar **Cadastros » Contas Caixa**, ou usar o **Busca Menu** digitando "conta caixa".
2. Ver o [[procedimentos/padrao-botoes-cadastro|padrão de botões e atalhos de cadastro]] (Inclusão, Alteração, Exclusão, Consulta, Lista, Pesquisa).
3. Ao incluir uma conta, definir se ela é uma conta pai ou uma conta filha (seguindo a estrutura da conta pai correspondente), e classificá-la como Débito ou Crédito.

## Campos e Parâmetros Importantes
- **Débito (D)**: contas usadas para saídas de valor do caixa — pagamentos, retiradas.
- **Crédito (C)**: contas usadas para entradas de valor no caixa — vendas, suprimentos, formas de pagamento recebidas.
- O cadastro de contas filhas sempre deve seguir a estrutura/numeração da conta pai correspondente.

## Erros Comuns / Pontos de Atenção
- Atenção na escolha entre Débito e Crédito ao cadastrar a conta: **uma vez que a conta tenha movimentação (lançamentos) vinculada a ela, não é mais possível alterar se é Débito ou Crédito.**

## Rotinas Relacionadas
- Relatório **Demonstração de Resultados (DRE)** — é montado inteiramente com base nas contas caixa cadastradas.
