---
id: ROT-cadastro-operadores
title: "Cadastro de Operadores de Caixa"
type: rotina
audience: all
modulos: ["windows/caixa", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Cadastro de Operadores de Caixa
    type: RELACIONA_COM
    to: Abertura de Caixa
  - from: Cadastro de Operadores de Caixa
    type: RELACIONA_COM
    to: Fechamento de Caixa
  - from: Cadastro de Operadores de Caixa
    type: RELACIONA_COM
    to: Relatórios Caixas em Aberto por Operador
  - from: Cadastro de Operadores de Caixa
    type: RELACIONA_COM
    to: Movimentos Fechamento de Caixa Financeiro
---

## Visão Geral
Cadastra o operador que será vinculado a um Usuário do sistema. O operador também precisa estar cadastrado como Cliente no sistema — essa vinculação é usada para tratar casos de quebra de caixa (gera um valor a receber do operador responsável) ou sobra de caixa (gera um crédito para o operador). O cadastro também identifica o operador do caixa para que o fechamento seja feito corretamente.

## Quem Usa
Setor administrativo da empresa, ou responsável pelo cadastro de novos funcionários.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Cadastros » Operadores**, ou usar o Busca Menu digitando "cadastro operadores".
2. Ver o [[procedimentos/padrao-botoes-cadastro|padrão de botões e atalhos de cadastro]] (Inclusão, Alteração, Exclusão, Consulta, Lista, Pesquisa).
3. Informar Código, Nome e o Usuário vinculado ao operador.

## Campos e Parâmetros Importantes
- Relação **1 para 1** entre Usuário e Operador: um mesmo usuário não pode estar vinculado a mais de um cadastro de operador. Se tentar, o sistema bloqueia com a mensagem *"Usuário já utilizado pelo operador [código] - [nome]"*.

## Erros Comuns / Pontos de Atenção
- O campo **Ativo** precisa estar marcado para que o operador possa ser utilizado.
- Se o funcionário for desligado da empresa, o operador deve ser **desativado, nunca excluído** — excluir impede a geração de relatórios retroativos sobre esse operador.

## Rotinas Relacionadas
- [[rotinas/abertura-de-caixa|Abertura de Caixa]] — o operador é vinculado à abertura do caixa.
- Fechamento de Caixa — o operador identifica quem está fechando o caixa.
- Relatórios Caixas em Aberto por Operador — usa o cadastro do operador para o relatório (também disponível no módulo Business).
- Movimentos Fechamento de Caixa Financeiro — exige informar o operador (também disponível no módulo Business).
