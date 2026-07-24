---
id: ROT-relatorios-livro-caixa
title: "Relatórios Livro Caixa"
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
  - from: Relatórios Livro Caixa
    type: RELACIONA_COM
    to: Lançamentos Avulsos de Caixa
  - from: Relatórios Livro Caixa
    type: RELACIONA_COM
    to: Consultas Livro Caixa
  - from: Relatórios Livro Caixa
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
---

## Visão Geral
Relatório que valida as entradas e saídas do caixa e mostra o saldo — tanto o **saldo atual** quanto o **saldo anterior** (do dia anterior). O saldo anterior de um dia sempre vira o saldo atual do dia seguinte (saldo em cascata).

## Quem Usa
Setor Financeiro/Administrativo, e o dono da empresa, para entender a situação do caixa.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Livro Caixa** (atalho Alt+X).

## Campos e Parâmetros Importantes
Dúvidas geralmente vêm de **lançamentos incorretos** no caixa (reflexo do dado, não da rotina em si).

## Erros Comuns / Pontos de Atenção
Principalmente **lançamentos avulsos feitos incorretamente**. Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/lançamentos-avulsos-caixa|Lançamentos Avulsos de Caixa]]
- [[rotinas/consultas-livro-caixa|Consultas Livro Caixa]]
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
