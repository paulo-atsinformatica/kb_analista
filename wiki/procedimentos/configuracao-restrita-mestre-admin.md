---
id: PROC-configuracao-restrita-mestre-admin
title: "Botão Configurar (engrenagem) — acesso restrito a MESTRE/ADMIN"
type: procedimento
audience: all
modulos: []
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations: []
---

## O que é
Muitas rotinas do sistema têm um botão de **engrenagem** (Configurar) na barra de botões da tela. Esse botão só pode ser acessado por um usuário com login **MESTRE** ou **ADMIN** — usuários comuns não conseguem abrir essa configuração.

## Quando usar
Sempre que uma rotina tiver um botão de engrenagem/Configurar, referenciar este procedimento em vez de repetir a explicação — e documentar apenas o que aquela configuração específica faz.

## Exemplos já documentados
- Controle de Caixa: Sangria e Suprimento — associa conta caixa a cada tipo de movimentação.
- Relatórios Demonstração de Resultados (DRE) — define as contas caixa usadas no DRE.
- Movimentos Liquidação Em Lote — define como o sistema gera lançamentos ao liquidar vários documentos (um lançamento único, um por documento, ou perguntar ao usuário), e se mantém observação/conta caixa do documento original.
