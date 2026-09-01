# Log de Sessões de Entrevista

> Cada sessão de entrevista deve acrescentar uma entrada aqui, começando com `## [YYYY-MM-DD]`.

## [2026-07-16] setup | Geração inicial da pasta
- **Tipo:** setup automático
- **Rotinas pré-carregadas:** 1549 (esqueleto, status draft/pendente)
- **Módulos pré-carregados:** 77 (74 da taxonomia oficial + 3 extras encontrados na wiki principal: outros/ferramentas-suporte, windows/balancas, windows/clientes)
- **Observações:** Pasta gerada a partir do estado atual de `wiki/rotinas/` e `wiki/modulos/` do projeto principal. Nenhuma entrevista realizada ainda.

## [2026-07-16] entrevista | Windows » Caixa — MÓDULO CONCLUÍDO
- **Módulos confirmados nesta sessão:** todos os 34 módulos pré-mapeados (Windows, Web, Mobile, ATS HUB, Independentes, NFCe)
- **Rotinas concluídas:** todas as 31 rotinas de Windows » Caixa (100%). Lista completa: Abertura de Caixa, Cadastro de Contas Caixa, Cadastro de Operadores de Caixa, Cadastro de Turnos, Cadastro de Usuários (toda a família Windows), Consultas Livro Caixa, Consultas Saldo Geral, Consultas Saldo das Contas, Controle de Caixa (Sangria e Suprimento), Fechamento de Caixa, Fluxo de Caixa, Lançamentos Avulsos de Caixa, Movimentos Caixa de Recebimento Completo (obsoleta), Movimentos Fechamento de Caixa Financeiro, Movimentos Inicia Saldo Filiais, Movimentos Transferência de Conta Caixa entre Filiais (obsoleta), Parâmetros Caixa, Período de Lançamento de Caixa, Relatórios Caixa Gerencial (Por Trimestre/Trimestral-Anual/do Dia/por Período), Relatórios Caixas em Aberto por Operador, Relatórios Demonstração de Resultados (DRE), Relatórios Fechamento de Caixa, Relatórios Livro Caixa, Relatórios Saldo Contas Analítico, Relatórios Saldo Contas Sintético, Relatórios Saldo Geral de Custos, Transferência de Caixa para Conta Bancária, Utilitários Elimina Movimentos de Caixa, Utilitários Reprocessa Saldos (Caixa)
- **Rotinas em andamento (retomar):** nenhuma — módulo 100% concluído
- **Próximo módulo sugerido:** Windows » Faturamento (431 rotinas pré-mapeadas)
- **Observações:**
  - Taxonomia de módulos foi bastante reestruturada antes da entrevista começar: removidos módulos duplicados/inexistentes (api, atsmais, dba, avulso, gadgets, web-cloud); movidos/renomeados vários sub-módulos; NFCe promovido a categoria própria com 4 sub-módulos.
  - Durante a entrevista de Windows » Caixa: 26 rotinas pré-mapeadas foram confirmadas como não pertencentes ao Caixa (23 mantidas em outros módulos, 3 apagadas por serem exclusivas); "Gestão de Centros de Custo" confirmada como inexistente em 5 módulos (confundida com "Cadastro Centro de Custo"); 8 rotinas identificadas como duplicatas do levantamento original (nomes "Movimentos X" ou variações repetindo rotinas já cadastradas) e mescladas/removidas, incluindo "Relatórios Fechamento de Caixas por Operador" (duplicata de "Relatórios Fechamento de Caixa").
  - "Cadastro de Usuários" confirmado pelo analista como existente em toda a família Windows (17 sub-módulos).
  - Windows » Business acumulou 29 rotinas confirmadas ao longo da entrevista (praticamente espelha as rotinas de Caixa) — ainda não entrevistado formalmente como módulo próprio, apenas confirmado item a item via as rotinas de Caixa.
  - "Fluxo de Caixa" e "Transferência de Caixa para Conta Bancária" foram corrigidas: pré-mapeadas em windows/bancos, mas na verdade só existem no Business (Fluxo de Caixa) ou não pertencem a Bancos (Transferência para Conta Bancária).
  - Duas rotinas classificadas como `audience: analyst` por serem críticas/irreversíveis, de uso exclusivo do suporte ATS: Utilitários Elimina Movimentos de Caixa e Utilitários Reprocessa Saldos (Caixa).
  - Rotinas que existem em 3+ módulos foram movidas para `wiki/rotinas/_compartilhadas/`.
  - Criados 3 procedimentos gerais reaproveitáveis: Busca Menu, padrão de botões/atalhos de cadastro, ressalva de que erros só ocorrem por problema pontual de versão.

## [2026-07-16] entrevista | Windows » Pagar (em andamento)
- **Módulos confirmados nesta sessão:** nenhum novo (todos já confirmados na sessão anterior)
- **Rotinas concluídas:** Cadastro Histórico Padrão, Cadastro de Fornecedores, Cadastro de Moedas (Cotações e Identificação), Consultas Contas Pagas, Consultas Contas a Pagar Analítica/Sintética/Saldos/no Mês, Consultas Gráfico Posição Contas a Pagar, Consultas Movimentação Por Fornecedor, Movimento Agrupamento de Documentos (Fatura), Movimentos Cruzamento de Contas, Movimentos Entrada de Documento Simples, Movimentos Entrada de Documentos Automática, Movimentos Estorno, Movimentos Geração de Previsões, Movimentos Liquidação Em Lote, Movimentos Liquidação Impressão de Recibos, Movimentos Liquidação Individual, Movimentos Liquidação com Cheques Pré Recebidos, Movimentos Prorrogação, Relatório de Contas Pagas, Relatório de Contas a Pagar Por NF Entrada, Relatórios Contas a Pagar / Cheques, Relatórios Contas a Pagar Analítico, Relatórios Contas a Pagar Saldo, Relatórios Contas a Pagar Sintético
- **Rotinas em andamento (retomar):** Relatórios Fluxo de Caixa Analítico — entrevista interrompida a pedido do analista antes da pergunta 1 (ver observações); retomar quando o analista voltar ao módulo Pagar
- **Rotinas puladas a pedido do analista (retomar depois):** Configurações Financeiras: Documentos a Pagar e Receber; Movimentos Borderôs (+ Emitidos, Cancelamento); Movimentos Emissão de Autorização de Pagamento (+ Automática, Cancelamento, Por Período, individual)
- **Observações:**
  - Windows/Faturamento (421 rotinas): feita apenas a revisão de existência (não o conteúdo) — ver commit "confirma existencia das 421 rotinas restantes". Confirmado que TODO o módulo Faturamento também existe no Business.
  - Durante a revisão de Windows/Faturamento: removidas 2 rotinas inexistentes (Atualização de Dados Tributários em Lote, Bloqueio e Liberação de Clientes) e 8 duplicatas do levantamento original.
  - Durante a entrevista de Windows/Pagar: removida 1 rotina inexistente (Consultas Financeiras e Gestão de Cheques, também não existe em Bancos) e 1 duplicata/confusão de nome (Contas a Pagar — Liquidação Simples, confundida com Movimentos Entrada de Documento Simples).
  - Cadastro de Fornecedores confirmado em 7 módulos (Faturamento, Pagar, OS, Business, ResulthEmissorNFe, RetaguardaECF, EntregasCs).
  - Movimentos Entrada de Documento Simples/Automática, Movimentos Estorno e Movimentos Liquidação Individual/Em Lote têm comportamento diferente por módulo: no Pagar tratam documento a pagar, no Receber tratam documento a receber.
  - Criado procedimento geral sobre o botão de engrenagem (Configurar) restrito a usuário MESTRE/ADMIN, aplicado a várias rotinas (Sangria/Suprimento, DRE, Liquidação Em Lote).
  - Das 3 rotinas de liquidação: Individual pode ser estornada pela rotina genérica de Estorno; Em Lote e Com Cheques Pré Recebidos têm estorno próprio na tela. Em Lote é a única que aceita "aproveitamento de crédito" como forma de pagamento; Com Cheques Pré Recebidos é a única que aceita cheque e cartão.
  - Windows » Business segue acumulando rotinas confirmadas via as entrevistas de Caixa e Pagar (47 até agora).
  - Movimentos Liquidação com Cheques Pré Recebidos, Movimentos Prorrogação e Relatórios Contas a Pagar Analítico confirmadas como existentes em 3 módulos (Pagar/Receber/Business) e movidas para `wiki/rotinas/_compartilhadas/`. No Receber, os nomes pré-mapeados eram diferentes ("Movimentos Liquidação Com Pré-datados", "Movimentos Prorrogação Individual", "Relatórios Analítico de Vencimentos") — marcados como a mesma rotina, com nota explicativa. "Movimentos Prorrogação Em Lote" (só existe no Receber) é rotina distinta, ainda não entrevistada.
  - Corrigida lacuna encontrada: "Movimentos Liquidação Individual" estava faltando na página do módulo `wiki/modulos/windows/contas-a-receber.md` apesar de já confirmada nas 3 módulos.
  - Correção de deslize do analista: em "Relatórios Contas a Pagar Saldo", "documentos a pagar do cliente" foi corrigido para "do fornecedor" (mesmo padrão de deslize já observado antes em outras rotinas do Pagar).
  - Verificação geral de duplicatas solicitada pelo analista: encontradas e corrigidas 2 duplicatas exatas por truncamento de slug no módulo Sped ("...F100" e "...Registro 1020" — ambas apareciam 2x na mesma seção do checklist e como 2 arquivos pendentes idênticos).
  - Módulo "Windows » ERP_Faturamento" (criado em outra sessão paralela em 2026-08-01) foi mesclado/descontinuado: o analista confirmou que não é um sistema separado, é o mesmo Windows » Faturamento. Removido `wiki/modulos/windows/erp-faturamento.md`.
  - A pedido do analista, revisão livre (fora da ordem padrão de módulo): "Cadastro de Produtos" entrevistada por completo, confirmada em 7 módulos (Faturamento, Materiais, Compras, OS, Business, RetaguardaECF, ResulthEmissorNFe) e movida para `_compartilhadas/`. "NFE Digitação/Emissão de NFE" revisada e complementada com o módulo ResulthEmissorNFe (agora 3 módulos: Faturamento, Business, ResulthEmissorNFe), também movida para `_compartilhadas/`.
  - "Cadastro de Tipos de Operação" revisada com o analista (sem alterações de conteúdo) — apenas corrigidos wikilinks quebrados apontando para as rotinas que foram movidas para `_compartilhadas/` nesta sessão.
  - A pedido do analista, adicionada relação entre "NFE Digitação/Emissão de NFE" e "Cadastro de Contas Caixa"/"Cadastro Centro de Custo" (podem ser usadas em conjunto na operação de emissão da nota) — relação incluída nos 3 arquivos.
  - "Relatórios Fluxo de Caixa Analítico" confirmada como não existente no módulo Pagar (mantida apenas no Receber, onde ainda está pendente).
  - "NFE Digitação/Emissão de NFE" revisitada por completo a pedido do analista: Como Usar reescrito com passo a passo manual detalhado (Tipo de Operação → Cliente → Vendedor → Prazo/Desconto/Transportadora opcionais → Itens → Faturar → tela Emissão Nota Fiscal → OK) e opções de importação; adicionado botão Configurar com acesso restrito a MESTRE/ADMIN; adicionadas relações com Cadastro de Produtos, Cadastro de Vendedores, Cadastro Formas de Pagamento e Cadastro de Prazos de Pagamento.

## [2026-08-24] entrevista | Módulos (visão geral) — Caixa, Business, Pagar, Receber, Bancos
- **Tipo:** entrevista sobre os módulos em si (O que é / Quem Usa / Relacionamento com outros módulos), a pedido do analista, fora da sequência normal de rotinas.
- **Módulos entrevistados:** Windows » Caixa, Windows » Business, Windows » Pagar, Windows » Receber, Windows » Bancos — todos com `status_entrevista: concluida`.
- **Observações:**
  - Criado procedimento geral `wiki/procedimentos/requisitos-minimos-desktop-windows.md`: todo módulo da categoria Windows requer Desktop com Windows 10+ (de preferência Windows 11), processador Intel i5 ou superior, mínimo 8GB RAM. Referenciado em Caixa, Business, Pagar, Receber e Bancos.
  - Confirmado pelo analista: os módulos **Faturamento, Caixa, Bancos, Pagar e Receber** formam o conjunto "ERP" e são basicamente sempre usados juntos (um depende do outro para gerir a empresa) — Caixa controla o saldo de onde saem/entram os valores de Pagar/Receber/Bancos.
  - **Business** é o módulo mais completo: reúne as funções de todos os outros módulos (não tem 100% das funções de cada um individualmente, mas cobre o conjunto). Público-alvo: toda a empresa. Teoricamente substitui o conjunto ERP — quem tem só Business não precisa dos módulos separados.

## [2026-08-01] entrevista | Windows » Faturamento — grupo Digitação/Emissão de Notas e Cadastros de Clientes
- **Módulos confirmados nesta sessão:** nenhum dos pré-mapeados revisado; 1 módulo novo identificado e confirmado — Windows » ERP_Faturamento (sistema Windows independente, relacionado ao Faturamento, porém mais completo).
- **Rotinas concluídas:** Cadastro de Tipos de Operação, NFE Digitação/Emissão de NFE (nome exibido ao usuário: "Digitação/Emissão de NF-e"), Movimentos Emissão de NF de Vários Pedidos, Cadastro de Clientes, Cadastro de Compradores, Cadastro de Vendedores, Cadastro de Prazos de Pagamento, Cadastro de Tipo de Venda, Classificação de Clientes.
- **Rotinas puladas a pedido do analista (retomar depois):** Manutenção de Tipo de Operação x Conta Contábil; Movimentos Emissão de NF - Emissão de NFe em lote; e, do grupo Cadastros de Clientes: Gestão de Clientes Inativos, Gestão de Limites e Crédito de Clientes, Liberação do cadastro do cliente, Ficha Cadastral, Cadastros Transferência de Clientes.
- **Observações:**
  - Duas duplicatas do levantamento original confirmadas e mescladas: "Emissão de NF-e — Procedimento Básico" (duplicata de NFE Digitação/Emissão de NFE) e "NF de varios pedidos" (duplicata de Movimentos Emissão de NF de Vários Pedidos).
  - "Cadastro de Tipos de Operação" teve o módulo Windows » OS removido da lista (pré-mapeado, mas não confirmado pelo analista); confirmado que existe em Faturamento e Livros Fiscais (usado em Notas Fiscais Emitidas).
  - "Cadastro de Prazos de Pagamento" e "Classificação de Clientes" foram confirmados também em módulos que não estavam pré-mapeados: Prazos de Pagamento agora inclui Windows » Pagar; Classificação de Clientes agora inclui Windows » Receber (ambos seguem o mesmo padrão do Cadastro de Clientes/Cadastro de Fornecedores).
  - Ponto de atenção geral capturado em Cadastro de Tipos de Operação: não alterar operações já em uso (nem tudo fica no histórico) — preferir criar uma nova operação para situações específicas.
  - Em NFE Digitação/Emissão de NFE: forma de diferenciar rejeição da SEFAZ (mensagem traz o nome da SEFAZ) de erro interno do sistema (mensagem não traz).
  - Em Cadastro de Prazos de Pagamento: diferença entre "Prazos" (até 12, intervalo variável entre eles) e "Parcelas" (mais parcelas possíveis, intervalo fixo).
  - Nota: a rotina "Movimentos Liquidação com Cheques Pré Recebidos" (Windows » Pagar), que estava em andamento de sessão anterior, foi concluída em paralelo em outra sessão (ver entrada acima) — não foi retomada nesta sessão.
  - Próximo passo sugerido: retomar o grupo de Cadastros de Clientes pendente em Windows » Faturamento.
