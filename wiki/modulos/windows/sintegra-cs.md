---
id: MOD-windows-sintegra-cs
title: "Windows » SintegraCs"
type: modulo
audience: all
modulos: ["windows/sintegra-cs"]
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
Módulo com uma única função: gerar o arquivo Sintegra do cliente.

[[procedimentos/requisitos-minimos-desktop-windows|Requisitos mínimos: Desktop Windows 10 ou superior (de preferência Windows 11), processador Intel i5 (ou similar/superior), mínimo 8 GB de RAM]].

## Quem Usa
Empresas que precisam gerar o arquivo Sintegra. Não é necessário caso o cliente já tenha acesso ao módulo **RetaguardaECF**, já que o Sintegra também pode ser gerado por lá.

## Rotinas deste módulo
- Cadastro de Usuários

## Relacionamento com outros módulos
Precisa dos outros módulos que geram as movimentações do sistema (ex: Faturamento) — o SintegraCs em si serve exclusivamente para emitir o arquivo Sintegra, nenhuma outra função. Relaciona-se também com o **RetaguardaECF**, que pode gerar o Sintegra alternativamente.
