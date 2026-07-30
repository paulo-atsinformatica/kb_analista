---
id: ROT-movimentos-entrada-de-documento-simples
title: "Movimentos Entrada de Documento Simples"
type: rotina
audience: all
modulos: ["windows/contas-a-pagar", "windows/contas-a-receber", "windows/business"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Movimentos Entrada de Documento Simples
    type: RELACIONA_COM
    to: Cadastro de Fornecedores
  - from: Movimentos Entrada de Documento Simples
    type: RELACIONA_COM
    to: Cadastro Histórico Padrão
  - from: Movimentos Entrada de Documento Simples
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
  - from: Movimentos Entrada de Documento Simples
    type: RELACIONA_COM
    to: Movimento Agrupamento de Documentos (Fatura)
---

## Visão Geral
Faz o lançamento de documentos a pagar de forma manual e individual.

> [!NOTE] Comportamento diferente por módulo
> A mesma rotina, quando acessada pelo módulo **Contas a Receber**, gera um documento **a receber** em vez de a pagar — o restante do funcionamento é equivalente.

## Quem Usa
Setor Financeiro, direcionado para contas a pagar (ou a receber, dependendo do módulo).

## Módulos onde esta rotina existe
- windows/contas-a-pagar
- windows/contas-a-receber
- windows/business

## Como Usar (passo a passo)
1. Acessar **Movimentos » Entrada de Documentos » Simples** (atalho Ctrl+F2), ou pelo ícone "Entrada Docs." na barra de ferramentas.
2. Filtrar o Fornecedor que irá receber o documento a pagar.
3. Informar o Tipo de Documento, número do documento, Data de Emissão e Vencimento, Valor do documento, Desconto ou Juros/Multas (se houver).
4. Informar o Histórico — pode ser um dos padrões cadastrados (ver [[rotinas/_compartilhadas/cadastro-historico-padrao|Cadastro Histórico Padrão]]) ou digitado manualmente.
5. Informar a Conta Caixa e, se necessário, o Centro de Custo.
6. Clicar em OK para gerar o documento.

## Campos e Parâmetros Importantes
Sem dúvidas — rotina simples de preencher.

## Erros Comuns / Pontos de Atenção
Ver [[procedimentos/erros-apenas-por-versao-com-problema|ressalva geral sobre erros]] — só ocorrem por problema pontual de versão.

## Rotinas Relacionadas
- [[rotinas/_compartilhadas/cadastro-fornecedores|Cadastro de Fornecedores]]
- [[rotinas/_compartilhadas/cadastro-historico-padrao|Cadastro Histórico Padrão]]
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]]
- Movimento Agrupamento de Documentos (Fatura)
