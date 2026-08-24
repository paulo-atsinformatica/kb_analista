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
data_atualizacao: 2026-08-24
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
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Cadastro de Produtos
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Cadastro de Vendedores
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Cadastro Formas de pagamento
  - from: NFE Digitação/Emissão de NFE
    type: RELACIONA_COM
    to: Cadastro de Prazos de Pagamento
---

> [!INFO] Nome exibido ao usuário
> Na tela do sistema, a rotina aparece como **"Digitação/Emissão de NF-e"**. Caminho: **NF-e » Digitação/Emissão de NF-e**.

## Visão Geral
Rotina utilizada para emitir NF-e/NFS-e (Nota Fiscal e Nota Fiscal de Serviço).

Pré-requisitos para emitir uma nota:
- Ter o **Tipo de Operação** cadastrado (define o CFOP, usado para indicar para qual estado ou finalidade é a nota).
- Ter o **Cliente** cadastrado, com as informações obrigatórias (e-mail, IE quando o cliente tiver, e o endereço do tipo **Nota Fiscal Eletrônica** cadastrado na aba de endereços).
- Informar o **Vendedor** (obrigatório).

## Quem Usa
Quem precisa emitir Notas Fiscais — pode envolver Financeiro, Fiscal, Contábil ou quem estiver fazendo a venda.

## Módulos onde esta rotina existe
- windows/faturamento
- windows/business
- windows/resulth-emissor-nfe

## Como Usar (passo a passo)
A rotina geralmente vem facilitada: todo campo em **negrito** na tela é obrigatório — só é possível salvar após o preenchimento desses campos. A tela é dividida em duas partes (Cabeçalho e Itens). Alternativamente, a nota pode ser preenchida por **Importação** (botão "Importar Documento"): Importar Pedidos (Tipos 51 e 55 — PDV), Importar Pré-Venda, Importar ECF/NFC-e/SAT, Importar Orçamento, Importar Transferência de Estoque, Importar Trocas (Com/Sem Docto. de Origem), Importar Serviços (Tipo 55).

Passo a passo manual:
1. Ter o **Tipo de Operação** cadastrado, com o CFOP marcado corretamente para o tipo de nota.
2. Informar o **Cliente** (cadastro deve estar padronizado e correto).
3. Informar o **Vendedor**.
4. Opcionalmente, informar o **Prazo** (forma de pagamento) da nota.
5. Opcionalmente, informar o **Desconto** (em % ou valor).
6. Opcionalmente, informar a **Transportadora**.
7. Na aba **Itens**, informar o Produto e a Quantidade — os dados tributários são puxados automaticamente do cadastro do produto (ou do Perfil de Imposto associado a ele), mas podem ser alterados manualmente se necessário.
8. Clicar em **Faturar** — abre a tela **Emissão Nota Fiscal** (abas Faturamento, Transportadora, Comentários), onde é possível informar um comentário (aparece nos Dados Adicionais), valor e forma de cobrança do frete, dados da transportadora/volumes, e a forma de pagamento (caso não tenha sido informada antes).
9. Clicar em **OK** para emitir a nota.

## Campos e Parâmetros Importantes
- O principal ponto de atenção é em relação ao **cálculo e destaque dos impostos**, que fica concentrado na parte de Itens.
- A rotina tem um botão de **Configurar**, com [[procedimentos/configuracao-restrita-mestre-admin|acesso restrito a MESTRE/ADMIN]], que abre a tela de parâmetros para a emissão da nota (ex: numeração da NF-e, empresa que gera caixa/NF de saída, decimais de preço/quantidade, comportamento em caso de estoque insuficiente, campos livres da NF-e, permissões de faturamento por usuário, entre outros).

## Erros Comuns / Pontos de Atenção
- **Rejeição da SEFAZ**: erro comum mais frequente — a mensagem de rejeição vem acompanhada do erro retornado pela SEFAZ. Quando a rejeição é da SEFAZ, a mensagem traz uma informação específica identificando a SEFAZ; quando o erro é do próprio sistema (não da SEFAZ), a mensagem **não** traz o nome da SEFAZ — isso ajuda a diferenciar rejeição fiscal de erro interno do sistema.
- **Valor de impostos incorreto na pré-emissão**: pode ser causado por configuração (ex: Tipo de Operação, cadastro tributário do produto) ou falta de valor/parâmetro configurado.
- Ponto de atenção geral: cuidado ao digitar o produto errado, ou informar valor ou tributação incorreta na nota.

## Rotinas Relacionadas
Relaciona-se com (rotinas independentes, não há dependência de execução entre elas):
- [[rotinas/cadastro-tipos-de-operacao|Cadastro de Tipos de Operação]] — toda nota exige uma operação cadastrada.
- [[rotinas/movimentos-entrada-de-produtos|Movimentos Entrada de Produtos]] — relacionada principalmente à nota de **devolução de compra**.
- Cadastro de Clientes — toda nota tem um cliente vinculado.
- [[rotinas/_compartilhadas/cadastro-produtos|Cadastro de Produtos]] — toda nota tem produto(s)/serviço(s) vinculado(s).
- [[rotinas/cadastro-vendedores|Cadastro de Vendedores]] — o vendedor é campo obrigatório na nota.
- [[rotinas/cadastro-formas-de-pagamento|Cadastro Formas de Pagamento]] e [[rotinas/cadastro-prazos-de-pagamento|Cadastro de Prazos de Pagamento]] — usados na forma/prazo de pagamento da nota.
- [[rotinas/_compartilhadas/cadastro-contas-caixa|Cadastro de Contas Caixa]] e [[rotinas/cadastro-centro-de-custo|Cadastro Centro de Custo]] — podem ser utilizadas em conjunto com a emissão da nota (informação de conta caixa e centro de custo na operação).
