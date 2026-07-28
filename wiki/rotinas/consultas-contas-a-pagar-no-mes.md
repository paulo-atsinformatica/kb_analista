---
id: ROT-consultas-contas-a-pagar-no-mes
title: "Consultas Contas a Pagar no Mês"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Consultas Contas a Pagar no Mês
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Analítica
  - from: Consultas Contas a Pagar no Mês
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Sintética
  - from: Consultas Contas a Pagar no Mês
    type: RELACIONA_COM
    to: Consultas Contas a Pagar Saldos
---

## Visão Geral
Mostra em formato de calendário os valores a pagar por dia do mês filtrado.

## Quem Usa
Setor Financeiro.

## Módulos onde esta rotina existe
- windows/contas-a-pagar

## Como Usar (passo a passo)
1. Acessar **Consultas » Contas a Pagar no Mês** (atalho Ctrl+C), ou pelo ícone "A pagar no Mês" na barra de ferramentas.

## Campos e Parâmetros Importantes
- Atenção ao filtro **Tipo de Documento**: se informar um tipo sem nenhum documento lançado, o resultado aparece vazio (esperado, não é erro do sistema).

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- Consultas Contas a Pagar Analítica
- Consultas Contas a Pagar Sintética
- Consultas Contas a Pagar Saldos
