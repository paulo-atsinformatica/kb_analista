---
id: ROT-cadastro-produtos
title: "Cadastro de Produtos"
type: rotina
audience: all
modulos: ["windows/faturamento", "windows/materiais", "windows/compras", "windows/os", "windows/business", "windows/retaguarda-ecf", "windows/resulth-emissor-nfe"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-08-19
fontes: []
entities: []
relations:
  - from: Cadastro de Produtos
    type: RELACIONA_COM
    to: Movimentos Entrada de Produtos
  - from: Cadastro de Produtos
    type: RELACIONA_COM
    to: NFE Digitação/Emissão de NFE
---

## Visão Geral
Rotina utilizada para cadastrar os produtos/serviços que serão utilizados no sistema, para vendas e prestações de serviço. Também é usada para outros tipos de cadastro de produto, como: Ativo Imobilizado, Embalagem, Mercadoria para Revenda, Uso e Consumo, Matéria-Prima, Outras, Outros Insumos, Produto Intermediário, Produto em Processo, Produto Acabado, Serviço e SubProduto.

## Quem Usa
Responsável pelos cadastros de produtos.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/materiais
- windows/compras
- windows/os
- windows/business
- windows/retaguarda-ecf
- windows/resulth-emissor-nfe

## Como Usar (passo a passo)
1. Acessar **Cadastros » Produtos » Produtos** (ou pelo ícone de produto no menu).
2. Pode-se usar o botão de **Clonagem** para clonar um produto já cadastrado (só é necessário alterar a descrição), ou fazer o cadastro manual, informando todos os campos em **negrito** (obrigatórios).
3. **Aba Dados Iniciais**: informar o Indicador do Produto (Terceiros/Importado/Próprio/Serviço), o Tipo do Produto (Ativo Imobilizado, Embalagem, Matéria-Prima, Mercadoria para Revenda, Uso e Consumo, Produto Acabado, Serviço, SubProduto, etc.), Referência (EAN), Ref. Fabricante, Grupo, Subgrupo, Marca, Família, Descrição (obrigatória), foto, Unidade de Entrada/Saída, se o produto é Fracionado e o Fator de Conversão.
4. **Aba Dados Tributários**: sub-abas Dados Principais (NCM, NBS para serviço, CSOSN, CEST se ICMS ST na entrada, PIS/COFINS), ICMS (alíquota, base e CST para vendas dentro do estado — vendas fora do estado configuram-se por região), Substituição Tributária (ICMS ST gerado na emissão de notas) e Perfil de Imposto (permite vincular um perfil já cadastrado ao invés de repetir a configuração tributária em cada produto).
5. **Aba Preços/Fornecedores**: cadastro dos valores de venda (até 4 preços de venda diferentes, preço promocional), com sub-aba Dados Estatísticos mostrando as últimas 3 notas de entrada do produto.
6. **Aba Campos Pessoais**: observações e campos adicionais customizáveis pelo cliente.
7. **Aba Aplicações** (se configurado): cadastro das aplicações do produto, usado na venda para identificar a aplicação correta.
8. **Aba Complementos**: informações específicas do produto (ex: dados de medicamento/ANVISA, combustíveis).

> [!IMPORTANT] Dados tributários são de responsabilidade da contabilidade
> Todos os dados da aba Dados Tributários devem ser passados diretamente pela contabilidade do cliente — não deve ser informado nenhum dado tributário por conta própria para o cliente.

## Campos e Parâmetros Importantes
- O botão de **Configurar** abre a tela **"Configurações de Produto"**, com diversos parâmetros que definem: campos obrigatórios (Repetir Referência, Repetir Referência do Fabricante, etc.), regras de cálculo de preço de venda/margem, regras dos 4 preços de venda (Obrigatório / Aceitar e avisar se for 0 / Aceitar sem avisar), decimais de preço e de custo, uso de dólar, exibição de foto na pesquisa, entre outros.
- O checkbox **Fracionado** precisa estar marcado para o produto aceitar quantidade quebrada (ex: 2,5 / 3,1) na venda — se não estiver marcado, o sistema não permite vender número quebrado.

## Erros Comuns / Pontos de Atenção
- Produto que deveria aceitar quantidade fracionada (ex: 2,5 kg) e não vende quebrado — verificar se o checkbox **Fracionado** está marcado.
- Não há muitos erros comuns fixos, pois a rotina é bem específica para cada tipo de produto.

## Rotinas Relacionadas
- [[rotinas/movimentos-entrada-de-produtos|Movimentos Entrada de Produtos]]
- [[rotinas/nfe-digitacaoemissao-de-nfe|NFE Digitação/Emissão de NFE]]
- Pré-Venda, Orçamento, Pedidos
- Relatórios de Movimentação que filtram por produto
- Curva ABC
- Basicamente todas as rotinas que envolvem produtos.
