---
id: ROT-nfe-digitacaoemissao-de-nfe
title: "NFE Digitação/Emissão de NFE"
type: rotina
audience: all
modulos: ["windows/faturamento", "windows/business", "windows/resulth-emissor-nfe"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-19
fontes: []
entities: []
relations:
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Cadastro de Tipos de Operação
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Movimentos Entrada de Produtos
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Cadastro de Clientes
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Cadastro de Contas Caixa
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Cadastro Centro de Custo
---

> [!INFO] Nome exibido ao usuário
> Na tela do sistema, a rotina aparece como **"Digitação/Emissão de NF-e"**. Caminho: **NF-e » Digitação/Emissão de NF-e**.

## Visão Geral
Rotina usada para emitir Notas Fiscais de produtos e/ou serviços.

## Quem Usa
Quem precisa emitir Notas Fiscais — pode envolver Financeiro, Fiscal, Contábil ou quem estiver fazendo a venda.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/business
- windows/resulth-emissor-nfe

## Como Usar (passo a passo)
A rotina geralmente vem facilitada: todo campo em **negrito** na tela é obrigatório — só é possível salvar após o preenchimento desses campos.

1. Na primeira tela (**Cabeçalho**), preencha os dados principais: Tipo de Operação, Cliente, Vendedor, forma de pagamento (existe uma tela de forma de pagamento mais completa antes de finalizar).
2. Na aba de **Itens**, informe o produto/serviço da nota, quantidade e os dados de impostos.
3. Após preencher as informações necessárias (obrigatórias ou não, dependendo do tipo de nota emitida), o botão **Faturar** é habilitado.
4. Ao clicar em **Faturar**, abre uma nova tela (**Emissão Nota Fiscal**) com as abas Faturamento, Transportadora e Comentários, onde se conclui a emissão.

## Campos e Parâmetros Importantes
O principal ponto de atenção é em relação ao **cálculo e destaque dos impostos**, que fica concentrado na parte de Itens.

## Erros Comuns / Pontos de Atenção
- **Valor de impostos incorreto na pré-emissão**: pode ser causado por configuração (ex: Tipo de Operação, cadastro tributário do produto) ou falta de valor/parâmetro configurado.
- **Rejeição da SEFAZ**: quando a nota é rejeitada pela SEFAZ por erro na nota, a mensagem retornada traz uma informação específica identificando a SEFAZ. Já quando o erro é do sistema (não da SEFAZ), a mensagem **não** traz o nome da SEFAZ — isso ajuda a diferenciar rejeição fiscal de erro interno do sistema.

## Rotinas Relacionadas
Relaciona-se com (rotinas independentes, não há dependência de execução entre elas):
- [[rotinas/cadastro-tipos-de-operacao|Cadastro de Tipos de Operação]] — toda nota exige uma operação cadastrada.
- [[rotinas/movimentos-entrada-de-produtos|Movimentos Entrada de Produtos]] — usada quando a nota emitida é uma devolução.
- Cadastro de Clientes — toda nota tem um cliente vinculado.
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]] e [[rotinas/cadastro-centro-de-custo|Cadastro Centro de Custo]] — podem ser utilizadas em conjunto com a emissão da nota (informação de conta caixa e centro de custo na operação).
