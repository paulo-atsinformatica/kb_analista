---
id: ROT-consultas-livro-caixa
title: "Consultas Livro Caixa"
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
  - from: Consultas Livro Caixa
    type: RELACIONA_COM
    to: Abertura de Caixa
  - from: Consultas Livro Caixa
    type: RELACIONA_COM
    to: Fechamento de Caixa
  - from: Consultas Livro Caixa
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
---

## Visão Geral
Consulta as movimentações (entradas e saídas) do caixa numa data ou período específico.

## Quem Usa
Pessoa do Financeiro, ou o próprio operador do caixa, para ter seus lançamentos em controle.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Consultas » Livro Caixa** (atalho Ctrl+L).
2. Informar o período que deseja consultar.
3. Escolher a ordem de exibição dos registros: Ordem natural de lançamento, Data/Conta Caixa, ou Data/Histórico.
4. Opcionalmente, incluir as colunas de Operador e Turno.

## Campos e Parâmetros Importantes
Sem dúvidas ou parâmetros específicos — só reflete erro se já houver alguma informação incorreta lançada no sistema.

## Erros Comuns / Pontos de Atenção
Sem erros específicos da rotina em si — problemas só aparecem se houver dado incorreto já lançado no sistema. Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/abertura-de-caixa|Abertura de Caixa]] — pode ser usada para conferência dos lançamentos.
- Fechamento de Caixa — pode ser usada para conferência dos lançamentos.
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]] — exibe os lançamentos por conta caixa.
