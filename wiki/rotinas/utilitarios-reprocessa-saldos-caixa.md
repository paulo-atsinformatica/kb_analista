---
id: ROT-utilitarios-reprocessa-saldos-caixa
title: "Utilitários Reprocessa Saldos (Caixa)"
type: rotina
audience: analyst
modulos: ["windows/caixa", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Utilitários Reprocessa Saldos (Caixa)
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
  - from: Utilitários Reprocessa Saldos (Caixa)
    type: RELACIONA_COM
    to: Consultas Saldo Geral
  - from: Utilitários Reprocessa Saldos (Caixa)
    type: RELACIONA_COM
    to: Consultas Saldo das Contas
---

> [!IMPORTANT] Rotina de suporte/manutenção
> Classificada como `audience: analyst` — envolve recálculo direto de saldos e é usada majoritariamente pelo suporte ATS/implantação, não pelo cliente final.

## Visão Geral
Faz o reprocessamento (recálculo) dos saldos do caixa. Geralmente utilizada quando há alguma divergência no saldo do caixa.

## Quem Usa
Suporte ATS ou equipe de implantação — pouco utilizada pelos clientes.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Utilitários » Reprocessa Saldos**.

## Campos e Parâmetros Importantes
Sem dúvidas registradas.

## Erros Comuns / Pontos de Atenção
- **Cuidado ao executar**: se feita de forma incorreta, pode alterar todo o saldo do cliente.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
- [[rotinas/consultas-saldo-geral|Consultas Saldo Geral]]
- [[rotinas/consultas-saldo-das-contas|Consultas Saldo das Contas]]
