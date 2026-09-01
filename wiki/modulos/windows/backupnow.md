---
id: MOD-windows-backupnow
title: "Windows » BackupNow"
type: modulo
audience: analyst
modulos: ["windows/backupnow"]
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
Sistema responsável por fazer o backup do banco de dados do sistema, de forma automática, salvando diretamente na nuvem da ATS. Uma vez cadastrados os dias e horários para o backup, ele é feito automaticamente desde que a máquina esteja ligada.

O BackupNow também aciona diretamente o suporte por e-mail caso o backup não seja realizado, e envia notificação (de sucesso ou de falha) para o e-mail do cliente ou para vários e-mails que podem ser cadastrados para receber esse aviso.

[[procedimentos/requisitos-minimos-desktop-windows|Requisitos mínimos: Desktop Windows 10 ou superior (de preferência Windows 11), processador Intel i5 (ou similar/superior), mínimo 8 GB de RAM]].

## Quem Usa
Não possui um público-alvo específico — serve para todos os sistemas e clientes.

## Rotinas deste módulo
> [!WARNING] Lista parcial
> Recuperada de um log de exclusão truncado — 12 de 14 rotinas originais. Confirmar com o analista se falta alguma.

- Backup Now - Backups - Backup Manual
- Backup Now - Backups - Configurar
- Backup Now - Backups - Dashboard
- Backup Now - Backups - Restaurar Backup
- Backup Now - Concluído com Sucesso
- Backup Now - Configurações - ATS Cloud
- Backup Now - Configurações - Atualizar Base de Dados do Sistema
- Backup Now - Configurações - Geral
- Backup Now - Configurações - Notificações
- Backup Now - Log
- Backup Now - Não Concluído
- Backup Now - Usuários
- Cadastro de Usuários

## Relacionamento com outros módulos
Independente — é específico para cuidar do banco de dados de todos os sistemas, sem depender de nenhum módulo em particular.
