---
id: ROT-parametros-caixa
title: "Parâmetros Caixa"
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
  - from: Parâmetros Caixa
    type: RELACIONA_COM
    to: Movimentos Inicia Saldo Filiais
  - from: Parâmetros Caixa
    type: RELACIONA_COM
    to: Período de Lançamento de Caixa
---

## Visão Geral
Rotina usada para configurar os parâmetros do módulo Caixa — as permissões/obrigações que regem o uso do sistema.

## Quem Usa
Equipe de Implantação, junto com o dono da empresa, durante a implantação/configuração do sistema.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. No módulo Caixa: acessar **Cadastros » Parâmetros**.
2. No Business: acessar **Cadastros » Parâmetros » Livro Caixa**.

## Campos e Parâmetros Importantes
- Cadastra as **contas caixa padrão** para vários tipos de movimentação: estorno de liquidações de contas a pagar/receber, estorno de vendas, devoluções, lançamento de excesso/falta no fechamento de caixa, cheques à vista/prazo.
- Configura o **período de lançamento automático** (mesma opção referenciada em Movimentos Inicia Saldo Filiais).
- Demais parâmetros variam conforme a regra de negócio de cada empresa: Integração Contábil, Informar Centro de Custo, Impressão do Fechamento de Caixa Financeiro, obrigar preencher turno na abertura, pedir empresa ao fazer lançamento, tolerância para fechamento de caixa, entre outros.

## Erros Comuns / Pontos de Atenção
Sem erros — rotina de configuração inicial, não é acessada durante o uso diário do sistema. Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/movimentos-inicia-saldo-filiais|Movimentos Inicia Saldo Filiais]]
- Período de Lançamento de Caixa — pode ser cadastrado automaticamente a partir daqui.
