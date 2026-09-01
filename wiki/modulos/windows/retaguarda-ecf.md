---
id: MOD-windows-retaguarda-ecf
title: "Windows » RetaguardaECF"
type: modulo
audience: all
modulos: ["windows/retaguarda-ecf"]
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
Módulo mais simples, geralmente utilizado junto com o **Resulth Checkout**. Serve para fazer o controle dos cadastros necessários para a emissão de NFC-e. Também tem a função de gerar o arquivo **Sintegra**, caso o cliente não tenha o módulo SintegraCs. É um módulo básico, que serve para controlar um pouco os relatórios de vendas e o controle dos operadores do Checkout.

[[procedimentos/requisitos-minimos-desktop-windows|Requisitos mínimos: Desktop Windows 10 ou superior (de preferência Windows 11), processador Intel i5 (ou similar/superior), mínimo 8 GB de RAM]].

## Quem Usa
Caso o cliente tenha apenas o Resulth Checkout, é utilizado por todos da empresa — por ser apenas um módulo necessário para os cadastros.

## Rotinas deste módulo
- Cadastro de Usuários
- Cadastro de Fornecedores
- Cadastro de Produtos

## Relacionamento com outros módulos
Geralmente utilizado junto com o **Resulth Checkout** (NFCe » Resulth Checkout). Também se relaciona com o **SintegraCs** — quando o cliente não tem o SintegraCs, é o RetaguardaECF que gera o arquivo Sintegra.
