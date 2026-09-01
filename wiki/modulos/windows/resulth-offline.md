---
id: MOD-windows-resulth-offline
title: "Windows » Resulth Offline"
type: modulo
audience: analyst
modulos: ["windows/resulth-offline"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-24
fontes: []
entities: []
relations: []
---

## O que é
Módulo que serve para integrar informações entre dois bancos de dados. Possui duas tratativas:

- **Integração entre Filiais**: integra informações de faturamento, produtos, clientes, entre outras, dependendo da regra de negócio — cada filial com o seu próprio banco.
- **Integração entre Caixa**: mais utilizada em supermercados. Cada caixa tem seu próprio banco, com um servidor centralizador. Diferente da integração por filial, aqui as vendas de cada caixa são integradas com um servidor da própria empresa — o que dá segurança: se o servidor tiver algum problema, a produção nos caixas não para; e se um caixa der problema, os demais continuam funcionando normalmente.

[[procedimentos/requisitos-minimos-desktop-windows|Requisitos mínimos: Desktop Windows 10 ou superior (de preferência Windows 11), processador Intel i5 (ou similar/superior), mínimo 8 GB de RAM]].

## Quem Usa
A tratativa de **integração entre caixas** é mais utilizada por **supermercados**. Já a **integração entre filiais** pode servir outros tipos de negócio, dependendo da regra de negócio do cliente.

## Rotinas deste módulo
- Cadastro de Usuários

## Relacionamento com outros módulos
Se relaciona com **Faturamento**, **Business** e **Caixa** — integra as informações de faturamento, produtos, clientes e vendas entre esses módulos e os bancos de dados envolvidos (filiais ou caixas).
