---
id: ROT-cadastro-historico-padrao
title: "Cadastro Histórico Padrão"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/bancos", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Cadastro Histórico Padrão
    type: RELACIONA_COM
    to: Lançamentos Avulsos de Caixa
  - from: Cadastro Histórico Padrão
    type: RELACIONA_COM
    to: Movimentos Entrada de Documento Simples
---

## Visão Geral
Cadastra históricos padrão que podem ser usados ao informar lançamentos de documentos ou lançamentos avulsos no sistema.

## Quem Usa
Setor Financeiro ou administrativo.

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/bancos
- windows/business

## Como Usar (passo a passo)
1. Acessar **Cadastros » Histórico Padrão**.
2. Clicar em Inclusão, informar a descrição que será o histórico (disponível depois em outras rotinas), e clicar em OK.

## Campos e Parâmetros Importantes
Sem campos/parâmetros especiais — rotina simples.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/lançamentos-avulsos-caixa|Lançamentos Avulsos de Caixa]] — usa o histórico cadastrado.
- Movimentos Entrada de Documento Simples — usa o histórico cadastrado (ex: PAGAMENTO DE TRANSPORTADORAS, PAGAMENTO FORNECEDORES). Basicamente toda rotina com campo Histórico usa esse cadastro.
