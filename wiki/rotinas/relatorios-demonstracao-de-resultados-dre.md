---
id: ROT-relatorios-demonstracao-de-resultados-dre
title: "Relatórios Demonstração de Resultados (DRE)"
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
  - from: Relatórios Demonstração de Resultados (DRE)
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
---

## Visão Geral
O DRE (Demonstração de Resultados) é o relatório onde são configuradas todas as contas caixa utilizadas pelo sistema. Serve para dar a demonstração mais exata dos resultados, uma vez configurado corretamente — mostra todos os lançamentos que geraram receita e despesa. Pode ser calculado tanto por **competência** quanto por **caixa**.

## Quem Usa
Geralmente o dono da empresa, para verificar se teve lucro ou não durante o período informado.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Relatórios » Demonstração de Resultados (DRE)**.
2. Selecionar Filiais e Período.
3. Selecionar os Centros de Custo (ou "Todos").
4. Escolher o cálculo do CMV (Preço de Custo, Preço Médio, ou Preço de Custo Atual).
5. Escolher o Tipo de Relatório/Regime: **Caixa** ou **Competência**.
6. Escolher o filtro por data: Pedido ou Faturamento.
7. Opcionalmente, marcar para imprimir apenas contas caixa com movimento, ou considerar movimentações bancárias originadas diretamente pelas filiais selecionadas.
8. Gerar o DRE.

## Campos e Parâmetros Importantes
- O botão de engrenagem (**Configurar** — ver [[procedimentos/configuracao-restrita-mestre-admin|acesso restrito a MESTRE/ADMIN]]) define as contas caixa usadas no DRE.
- A configuração do DRE geralmente é feita pela equipe de **Implantação**, após alinhar como funciona o fluxo do sistema e quais contas caixa são usadas.

## Erros Comuns / Pontos de Atenção
- Conta configurada **incorretamente** no DRE.
- Conta caixa nova cadastrada, mas **não associada ao DRE** — fica de fora do relatório.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
