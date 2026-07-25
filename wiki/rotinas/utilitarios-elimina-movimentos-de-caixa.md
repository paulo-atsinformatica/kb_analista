---
id: ROT-utilitarios-elimina-movimentos-de-caixa
title: "Utilitários Elimina Movimentos de Caixa"
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
  - from: Utilitários Elimina Movimentos de Caixa
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
  - from: Utilitários Elimina Movimentos de Caixa
    type: RELACIONA_COM
    to: Consultas Livro Caixa
  - from: Utilitários Elimina Movimentos de Caixa
    type: RELACIONA_COM
    to: Utilitários Reprocessa Saldos (Caixa)
---

> [!DANGER] Rotina crítica e irreversível
> Classificada como `audience: analyst` — apaga permanentemente movimentos do caixa. Uso exclusivo com suporte ATS; se usada incorretamente, não há como reverter.

## Visão Geral
Apaga os saldos/movimentos do caixa no período informado. Rotina deve ser usada exclusivamente com o suporte ATS, pois se usada incorretamente **não há como reverter**.

## Quem Usa
Suporte ATS.

## Módulos onde esta rotina existe
- windows/caixa
- windows/business

## Como Usar (passo a passo)
1. Acessar **Utilitários » Elimina Movimentos de Caixa**.
2. Informar o Período (data início e fim) a eliminar.
3. Confirmar em "Eliminar" — o sistema solicita login (Usuário/Senha) antes de executar.

## Campos e Parâmetros Importantes
- Exige senha de permissão para executar — só funciona com login **MESTRE**, **ADMIN**, ou usuário com permissão de **gerente**.

## Erros Comuns / Pontos de Atenção
- **Irreversível**: uma vez eliminados, os movimentos não podem ser recuperados.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
- [[rotinas/consultas-livro-caixa|Consultas Livro Caixa]]
- [[rotinas/utilitarios-reprocessa-saldos-caixa|Utilitários Reprocessa Saldos (Caixa)]]
