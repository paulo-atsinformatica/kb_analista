---
id: ROT-cadastro-fornecedores
title: "Cadastro de Fornecedores"
type: rotina
audience: all
modulos: ["windows/faturamento", "windows/contas-a-pagar", "windows/os", "windows/business", "windows/resulth-emissor-nfe", "windows/retaguarda-ecf", "windows/entregas-cs"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Cadastro de Fornecedores
    type: RELACIONA_COM
    to: Entrada de Produtos
---

## Visão Geral
Cadastra e consulta fornecedores — mostra histórico e movimentações do fornecedor. O cadastro pode ser feito manualmente ou consultando o CNPJ, que preenche as informações automaticamente.

## Quem Usa
Financeiro/Administrativo, principalmente usuários responsáveis por entrada de notas e contas a pagar.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/contas-a-pagar
- windows/os
- windows/business
- windows/resulth-emissor-nfe
- windows/retaguarda-ecf
- windows/entregas-cs

## Como Usar (passo a passo)
1. Acessar pelo ícone direto na barra de ferramentas, ou por **Cadastros » Fornecedor » Fornecedor** (atalho Ctrl+F).
2. Preencher manualmente, ou consultar pelo CNPJ para preenchimento automático.

## Campos e Parâmetros Importantes
- Existem parâmetros para bloquear ou avisar sobre **CNPJ/CPF** ou **IE (Inscrição Estadual)** duplicados.
- Para emitir **Notas de Devolução de Compras**, o fornecedor precisa também estar cadastrado como **cliente**, com os dois cadastros associados.

> [!NOTE] Observação interna (não repassar ao cliente)
> Se o servidor da ATS estiver fora do ar, a consulta por CNPJ falha e o sistema mostra a mensagem "CNPJ não foi localizado" — mesma mensagem exibida quando o CNPJ realmente não existe. Internamente, isso pode indicar instabilidade do servidor ATS, não necessariamente erro do usuário.

## Erros Comuns / Pontos de Atenção
- **CNPJ inválido** — quando o CNPJ informado está incorreto.
- **CNPJ não localizado** — CNPJ não encontrado na consulta (ou servidor ATS indisponível, ver nota interna acima).
- **IE inválida** — quando a Inscrição Estadual é obrigatória e está incorreta.

## Rotinas Relacionadas
- Entrada de Produtos
