---
id: ROT-cadastro-vendedores
title: "Cadastro de Vendedores"
type: rotina
audience: all
modulos: ["windows/faturamento", "windows/os"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Cadastro de Vendedores
    type: RELACIONA_COM
    to: Comissões de Vendedores
  - from: Cadastro de Vendedores
    type: RELACIONA_COM
    to: Cadastro de Metas por Grupo de Produtos
  - from: Cadastro de Vendedores
    type: RELACIONA_COM
    to: NFE Digitação/Emissão de NFE
  - from: Cadastro de Vendedores
    type: RELACIONA_COM
    to: Movimentos Pré-venda
  - from: Cadastro de Vendedores
    type: RELACIONA_COM
    to: Movimentos PDV
---

## Visão Geral
Rotina para cadastrar e identificar um vendedor.

## Quem Usa
Setor de Vendas ou Gestores.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/os

## Como Usar (passo a passo)
Caminho: **Cadastros » Vendedores » Vendedores**.

Rotina simples: preencher os campos obrigatórios (sinalizados em negrito, necessários para identificação) e salvar (Inclusão). Entre os campos: Nome, Filial, Tipo Pessoa/CNPJ-CPF, endereço, Comissão, Rotas (até 10), Tipo Vendedor (Vendedor/Atendente/Colaboradores/Supervisor/Preposto), Vendedor Responsável, Supervisor.

## Campos e Parâmetros Importantes
Nenhum ponto de atenção específico.

## Erros Comuns / Pontos de Atenção
Rotina simples, sem erros comuns registrados.

## Rotinas Relacionadas
- Comissões de Vendedores
- Cadastro de Metas por Grupo de Produtos
- [[rotinas/nfe-digitacaoemissao-de-nfe|NFE Digitação/Emissão de NFE]]
- [[rotinas/movimentos-pre-venda|Movimentos Pré-venda]]
- [[rotinas/movimentos-pdv|Movimentos PDV]]
- Ordem de Serviço (O.S.)
