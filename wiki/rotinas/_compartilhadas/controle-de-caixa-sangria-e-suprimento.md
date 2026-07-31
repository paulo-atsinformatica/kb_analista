---
id: ROT-controle-de-caixa-sangria-e-suprimento
title: "Controle de Caixa: Sangria e Suprimento"
type: rotina
audience: all
modulos: ["windows/caixa", "windows/business", "nfce/resulth-checkout"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Controle de Caixa: Sangria e Suprimento
    type: RELACIONA_COM
    to: Abertura de Caixa
  - from: Controle de Caixa: Sangria e Suprimento
    type: RELACIONA_COM
    to: Fechamento de Caixa
  - from: Controle de Caixa: Sangria e Suprimento
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
  - from: Controle de Caixa: Sangria e Suprimento
    type: RELACIONA_COM
    to: Cadastro de Operadores de Caixa
  - from: Controle de Caixa: Sangria e Suprimento
    type: RELACIONA_COM
    to: Cadastro de Turnos
  - from: Controle de Caixa: Sangria e Suprimento
    type: RELACIONA_COM
    to: Movimentos Lançamentos (Caixa)
---

## Visão Geral
Rotina utilizada para fazer lançamentos no caixa: de **saída** (Sangria) ou de **entrada** (Suprimento). Suprimentos geralmente são valores de troco; sangrias geralmente são quebras de caixa.

## Quem Usa
Principalmente o operador do caixa, que controla o valor necessário de entrada ou saída do caixa.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business
- nfce/resulth-checkout

## Como Usar (passo a passo)
1. Acessar **Movimentos » Lançamento de Sangria/Suprimento**, ou via Busca Menu.
2. Na inclusão, selecionar o **Tipo de movimento**: Sangria ou Suprimento.
3. Informar Empresa, Operador, Turno, Valor e Motivo. A Data e Hora são preenchidas automaticamente pelo sistema (puxadas da própria máquina), para evitar divergência no caixa.
4. Optar por imprimir o recibo da movimentação, para ser conferido pelo gerente ou administrativo no fechamento do caixa.

## Campos e Parâmetros Importantes
- O botão de engrenagem (**Configurar** — ver [[procedimentos/configuracao-restrita-mestre-admin|acesso restrito a MESTRE/ADMIN]]) permite associar uma conta caixa a cada tipo de movimentação (Sangria/Suprimento), necessário para que os relatórios de lançamentos saiam corretos.

## Erros Comuns / Pontos de Atenção
- Sempre solicitar a **impressão do recibo**, como comprovação de que o movimento foi feito.

## Rotinas Relacionadas
- [[rotinas/abertura-de-caixa|Abertura de Caixa]]
- Fechamento de Caixa
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
- [[rotinas/cadastro-operadores|Cadastro de Operadores de Caixa]]
- [[rotinas/_compartilhadas/cadastro-turnos|Cadastro de Turnos]]
- Movimentos Lançamentos (Caixa)
