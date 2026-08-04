---
id: ROT-cadastro-clientes
title: "Cadastro de Clientes"
type: rotina
audience: all
modulos: ["windows/faturamento", "windows/contas-a-receber"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-01
fontes: []
entities: []
relations:
  - from: Cadastro de Clientes
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
---

## Visão Geral
Rotina para identificar os dados cadastrais do cliente: nome, tipo de cliente, CPF ou CNPJ, endereço, etc. Também guarda o histórico de movimentação do cliente (compras, liquidações, etc.).

## Quem Usa
Vendedores, Financeiro, Gestores.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/contas-a-receber

## Como Usar (passo a passo)
Caminho: **Cadastros » Clientes » Clientes**.

O usuário preenche os dados nas abas (Dados Iniciais, Complementares, Cobrança/Entrega/NF-e, Contatos, Histórico). Os campos obrigatórios ficam sinalizados em **negrito** — só é possível salvar (Inclusão) após preenchê-los.

## Campos e Parâmetros Importantes
Rotina simples, sem pontos de atenção específicos além dos campos obrigatórios.

## Erros Comuns / Pontos de Atenção
- **CPF/CNPJ inválido**: o próprio sistema valida e informa quando o documento é inválido.
- **Cliente duplicado**: existe um parâmetro para bloquear ou permitir cadastro duplicado por CPF/CNPJ. O padrão do sistema é **não permitir** — o sistema informa que já existe cadastro com aquele CPF/CNPJ.

## Rotinas Relacionadas
Relaciona-se com todas as rotinas que precisam de um cliente vinculado (emissão de notas, pedidos, financeiro, etc.). Também se relaciona com [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]] — cliente e fornecedor permitem vínculo e reaproveitamento de informações de cadastro um do outro.
