---
id: ROT-movimentos-inicia-saldo-filiais
title: "Movimentos Inicia Saldo Filiais"
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
  - from: Movimentos Inicia Saldo Filiais
    type: RELACIONA_COM
    to: Período de Lançamento de Caixa
  - from: Movimentos Inicia Saldo Filiais
    type: RELACIONA_COM
    to: Parâmetros Caixa
---

## Visão Geral
Rotina usada para dar início ao saldo do caixa da filial — ou seja, quando o caixa da empresa foi iniciado e qual o saldo de abertura. Também cadastra o **período de lançamento**, que é o intervalo em que é possível fazer vendas e entradas no caixa da filial.

## Quem Usa
Geralmente configurada pela equipe de implantação, junto com o dono da empresa, durante o processo de implantação do sistema.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Inicia Saldo Filiais**.

## Campos e Parâmetros Importantes
- O saldo inicial só pode ser **alterado** se ainda não houver movimentação na filial. Se já houver movimento e tentar alterar, o sistema bloqueia com a mensagem: *"Saldo inicial não pode ser alterado pois existem movimentos para esta empresa!"*

## Erros Comuns / Pontos de Atenção
- Erro comum: cadastrar um **período curto** (poucos meses/dias), o que faz o período de lançamento expirar — exigindo lançar um novo período pela rotina Movimentos » Período de Lançamento. Recomendação: sempre colocar a data final com um período maior, para manter o lançamento liberado.
- Também é possível configurar em **Parâmetros » Caixa** para que o período seja atualizado automaticamente.

## Rotinas Relacionadas
- Período de Lançamento de Caixa
- Parâmetros Caixa
