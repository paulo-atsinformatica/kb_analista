---
id: ROT-abertura-de-caixa
title: "Abertura de Caixa"
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
  - from: Abertura de Caixa
    type: RELACIONA_COM
    to: Pré-venda (Orçamentos)
---

## Visão Geral
Rotina utilizada para abrir o caixa para o vendedor/operador. Deve ser informada a empresa, o usuário (vendedor/operador de caixa), o turno, a data e hora de abertura, e o valor em dinheiro liberado para a abertura. Por padrão, ao clicar em Inclusão (ou apertar F2), o sistema preenche automaticamente a data e a hora de abertura.

## Quem Usa
Operadores de caixa, administrativos e vendedores.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business — se o cliente tiver o módulo Fatura, precisa ter o módulo Caixa; se tiver apenas o Business, não precisa do Caixa.

## Como Usar (passo a passo)
1. Acessar o sistema Caixa informando usuário, senha e filial (a data de acesso é a data do movimento).
2. Ir em **Movimentos » Abertura de Caixa**, ou usar o **Busca Menu** digitando "abertura de caixa" (só aparece se o sistema estiver configurado para trabalhar com abertura de caixa e o usuário tiver permissão de acesso).
3. Preencher Empresa, Usuário, Turno, Data/Hora de abertura (preenchidas automaticamente) e Valor liberado.

## Campos e Parâmetros Importantes
- O acesso a esta rotina é restrito por permissão — geralmente configurado pelo gerente, já que complementa configurações gerais da empresa. A configuração deve ser alinhada com o dono do negócio para ficar fixa.
- Apenas usuários que **faturam vendas** precisam abrir caixa. Em um cenário com balcão de vendedores + caixa: só o operador do caixa (que fatura) precisa abrir caixa; vendedores que não faturam devem ter a permissão de faturar desabilitada, dispensando a abertura.

## Erros Comuns / Pontos de Atenção
- **Turno incorreto ou não informado**: o principal erro. O turno informado na abertura precisa ser o mesmo usado no fechamento de caixa — se estiver errado ou ausente, gera problema no fechamento.
- Sempre prestar atenção à **empresa** e ao **usuário** que está abrindo o caixa, para evitar abertura na empresa ou usuário errado.
- Se um usuário com permissão de faturar tentar iniciar uma venda (ex: Pré-venda/PDV) sem ter aberto o caixa, o sistema bloqueia com a mensagem: *"Caixa não aberto para esse usuário. É necessário a abertura de caixa pois o usuário possui permissão para faturar."*

## Rotinas Relacionadas
- [[rotinas/movimentos-vendas-pre-venda|Pré-venda (Orçamentos)]] — usuários com permissão de faturar precisam ter o caixa aberto antes de faturar uma venda; caso contrário, o sistema bloqueia a operação solicitando a abertura.
