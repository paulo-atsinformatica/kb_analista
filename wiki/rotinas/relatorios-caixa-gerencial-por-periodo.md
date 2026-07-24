---
id: ROT-relatorios-caixa-gerencial-por-periodo
title: "Relatórios Caixa Gerencial por Período"
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
  - from: Relatórios Caixa Gerencial por Período
    type: RELACIONA_COM
    to: Relatórios Caixa Gerencial do Dia
  - from: Relatórios Caixa Gerencial por Período
    type: RELACIONA_COM
    to: Relatórios Caixa Gerencial Por Trimestre
  - from: Relatórios Caixa Gerencial por Período
    type: RELACIONA_COM
    to: Relatórios Caixa Gerencial Trimestral/Anual
  - from: Relatórios Caixa Gerencial por Período
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
---

## Visão Geral
Gera o saldo geral dos caixas, agrupado pelas contas caixa, num intervalo de período. Pode ser agrupado em 3 níveis, seguindo a hierarquia da conta:
- **Nível 1**: contas caixa pelos primeiros 2 dígitos (ex: `02`, `03`, `04`).
- **Nível 2**: contas caixa com 4 dígitos (ex: `0201`, `0204`, `0207`).
- **Nível 3**: conta completa, 7 dígitos (ex: `0201001`).

## Quem Usa
Dono da empresa, ou administrativo/financeiro.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Relatório Gerencial de Caixa » Caixa Gerencial por Período**.
2. Informar o período desejado e o nível de agrupamento (1, 2 ou 3).

## Campos e Parâmetros Importantes
Ver a explicação dos níveis de agrupamento acima — é o ponto mais importante da rotina.

## Erros Comuns / Pontos de Atenção
Sem erros — relatório tranquilo de gerar. Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/relatorios-caixa-gerencial-do-dia|Relatórios Caixa Gerencial do Dia]]
- [[rotinas/relatorios-caixa-gerencial-por-trimestre|Relatórios Caixa Gerencial Por Trimestre]]
- [[rotinas/relatorios-caixa-gerencial-trimestralanual|Relatórios Caixa Gerencial Trimestral/Anual]]
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
