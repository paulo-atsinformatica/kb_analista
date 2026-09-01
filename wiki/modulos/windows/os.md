---
id: MOD-windows-os
title: "Windows » Ordem de Serviço"
type: modulo
audience: all
modulos: ["windows/os"]
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
Módulo à parte do sistema, utilizado para gerar Ordens de Serviço — desde aparelhos até auto peças, mais usado em oficinas onde o serviço é prestado. A OS gera o pedido que será faturado e a nota emitida pelo Business ou pelo Faturamento.

> [!IMPORTANT] Base de dados integrada, mas separada
> A OS possui uma base de dados própria, integrada com a base principal. Ao aplicar uma atualização no sistema, além da base principal, a OS também deve ser aberta separadamente para que a sua própria base seja atualizada.

[[procedimentos/requisitos-minimos-desktop-windows|Requisitos mínimos: Desktop Windows 10 ou superior (de preferência Windows 11), processador Intel i5 (ou similar/superior), mínimo 8 GB de RAM]].

## Quem Usa
Setor Financeiro e setor de Operação — os serviços e peças utilizados no atendimento são lançados na OS.

## Rotinas deste módulo
- Cadastro Atendimento
- Cadastro Atividade
- Cadastro Cargos
- Cadastro Categorias
- Cadastro Causas de Defeitos
- Cadastro Combustíveis
- Cadastro Cores
- Cadastro Defeitos
- Cadastro Itens Para Check-List
- Cadastro Marcas/Modelos
- Cadastro Modelos
- Cadastro Motivos de Cancelamentos
- Cadastro Motivos de Devoluções
- Cadastro Motivos de Paralisações/Suspensões
- Cadastro Motivos de Recusas
- Cadastro Prismas
- Cadastro Relação Defeitos X Causas
- Cadastro Relação Defeitos X Causas X Serviços
- Cadastro Relação Serviços X Peças
- Cadastro de Aplicações de Produtos
- Cadastro de Categorias de Equipamentos (OS)
- Cadastro de Colaboradores (OS)
- Cadastro de Código de Serviço (NFS-e)
- Cadastro de Fornecedores
- Cadastro de Marcas
- Cadastro de Motivos (OS)
- Cadastro de Motivos de Cancelamento
- Cadastro de Motivos de Devolução
- Cadastro de Motivos de Paralisação/Suspensão
- Cadastro de Motivos de Recusa
- Cadastro de Produtos
- Cadastro de Seguradoras
- Cadastro de Serviços
- Cadastro de Situações de Equipamentos
- Cadastro de Tipos de Atendimento (OS)
- Cadastro de Tipos de Operação
- Cadastro de Usuários
- Cadastro de Vendedores
- Cadastros Dados Complementares
- Contratos Apólice Seguro de Equipamentos
- Contratos Apólice Seguro de Veículos
- Contratos Licitação
- Contratos Manutenção de Equipamentos
- Contratos Manutenção de Veículos
- Devolver Peças
- Gestão de Contratos de Licitação
- Gestão de Licitações
- Movimentação Acompanhamento O.S.
- Movimentação Acompanhamento Requisição
- Movimentação Acompanhamento Revisão
- Movimentação Apontamento de Tempos Veículo
- Movimentação O.S. Equipamentos Abrir
- Movimentação O.S. Equipamentos Alocar Mão-de-Obra
- Movimentação O.S. Equipamentos Aprovar/Recusar Orçamento
- Movimentação O.S. Equipamentos Aproveita Orçamento Vencido
- Movimentação O.S. Equipamentos Cancelar Encerramento
- Movimentação O.S. Equipamentos Cancelar O.S.
- Movimentação O.S. Equipamentos Devolver Peças
- Movimentação O.S. Equipamentos Encerrar
- Movimentação O.S. Equipamentos Fechar
- Movimentação O.S. Equipamentos Iniciar
- Movimentação O.S. Equipamentos Paralisar
- Movimentação O.S. Equipamentos Reiniciar
- Movimentação O.S. Veículos Abrir
- Movimentação O.S. Veículos Alocar Mão-de-Obra
- Movimentação O.S. Veículos Aprovar/Recusar Orçamento
- Movimentação O.S. Veículos Aproveitar Orçamento Vencido
- Movimentação O.S. Veículos Cancela Encerramento
- Movimentação O.S. Veículos Cancela O.S.
- Movimentação O.S. Veículos Encerrar
- Movimentação O.S. Veículos Fechar
- Movimentação O.S. Veículos Iniciar
- Movimentação O.S. Veículos Paralisar
- Movimentação O.S. Veículos Reiniciar
- Movimentação Requisições  Abrir
- Movimentação Requisições Aprovar/Recusar
- Movimentação Requisições Baixar
- Movimentação Requisições Cancelar
- Movimentação Requisições Cancelar Baixa
- Movimentação Requisições Devolver Peças
- Ordem de Serviço (O.S.)
- Ordem de Serviço (OS)
- Parâmetros Ordem de Serviço (O.S.)
- Relatórios Comissões (O.S.)
- Relatórios Duração de Etapas da O.S.
- Relatórios Log do Sistema
- Relatórios O.S. Canceladas/Paralisadas/Recusadas
- Relatórios O.S. Equipamento Serviços/Peças
- Relatórios O.S. Equipamentos
- Relatórios O.S. Veículos
- Relatórios O.S. Veículos Serviços/Peças
- Relatórios Produtividade e Tempos de Serviços
- Rotina: Cálculo e Relatórios de Comissões
- Utilitários Backup/Limpeza do Log
- Utilitários Limpa Movimentações
- Utilitários Recalcular estoque bloqueado
- Utilitários Recria Base Dados

## Relacionamento com outros módulos
Pode ser utilizado tanto com o **Business** quanto com o **Faturamento** — é para um desses dois módulos que o pedido gerado na OS é faturado e a nota emitida.
