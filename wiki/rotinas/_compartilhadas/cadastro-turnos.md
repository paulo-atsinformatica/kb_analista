---
id: ROT-cadastro-turnos
title: "Cadastro de Turnos"
type: rotina
audience: all
modulos: ["windows/caixa", "windows/faturamento", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Cadastro de Turnos
    type: RELACIONA_COM
    to: Abertura de Caixa
  - from: Cadastro de Turnos
    type: RELACIONA_COM
    to: Fechamento de Caixa
  - from: Cadastro de Turnos
    type: RELACIONA_COM
    to: Movimentos Fechamento de Caixa Financeiro
---

## Visão Geral
Cadastra os turnos que serão utilizados na abertura do caixa. É informada a descrição do turno e o intervalo de horário que ele compreende.

## Quem Usa
Gestão da empresa — define os horários dos turnos de trabalho.

## Módulos onde esta rotina existe
- windows/caixa
- windows/faturamento
- windows/business

## Como Usar (passo a passo)
1. Acessar **Cadastros » Turnos**.
2. Ver o [[procedimentos/padrao-botoes-cadastro|padrão de botões e atalhos de cadastro]] (Inclusão, Alteração, Exclusão, Consulta, Lista, Pesquisa).
3. Informar a descrição do turno (ex: "Manhã 08:00 às 12:00", "Tarde 13:00 às 18:00"). A definição dos turnos fica a critério do gestor da empresa.

## Campos e Parâmetros Importantes
Sem dúvidas registradas para este cadastro.

## Erros Comuns / Pontos de Atenção
Sem erros comuns registrados para este cadastro. Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/abertura-de-caixa|Abertura de Caixa]] — exige informar o turno.
- Fechamento de Caixa — exige informar o turno (deve ser o mesmo da abertura).
- Movimentos Fechamento de Caixa Financeiro — exige informar o turno.
