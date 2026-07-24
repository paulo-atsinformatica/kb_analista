# Log de Sessões de Entrevista

> Cada sessão de entrevista deve acrescentar uma entrada aqui, começando com `## [YYYY-MM-DD]`.

## [2026-07-16] setup | Geração inicial da pasta
- **Tipo:** setup automático
- **Rotinas pré-carregadas:** 1549 (esqueleto, status draft/pendente)
- **Módulos pré-carregados:** 77 (74 da taxonomia oficial + 3 extras encontrados na wiki principal: outros/ferramentas-suporte, windows/balancas, windows/clientes)
- **Observações:** Pasta gerada a partir do estado atual de `wiki/rotinas/` e `wiki/modulos/` do projeto principal. Nenhuma entrevista realizada ainda.

## [2026-07-16] entrevista | Windows » Caixa
- **Módulos confirmados nesta sessão:** todos os 34 módulos pré-mapeados (Windows, Web, Mobile, ATS HUB, Independentes, NFCe)
- **Rotinas concluídas:** Abertura de Caixa, Cadastro de Contas Caixa, Cadastro de Operadores de Caixa, Cadastro de Turnos, Cadastro de Usuários (toda a família Windows), Consultas Livro Caixa, Consultas Saldo Geral, Consultas Saldo das Contas, Controle de Caixa (Sangria e Suprimento), Fechamento de Caixa, Fluxo de Caixa, Lançamentos Avulsos de Caixa, Movimentos Caixa de Recebimento Completo (obsoleta), Movimentos Fechamento de Caixa Financeiro, Movimentos Inicia Saldo Filiais, Movimentos Transferência de Conta Caixa entre Filiais (obsoleta), Parâmetros Caixa, Período de Lançamento de Caixa, Relatórios Caixa Gerencial Por Trimestre/Trimestral-Anual/do Dia/por Período, Relatórios Caixas em Aberto por Operador, Relatórios Demonstração de Resultados (DRE), Relatórios Fechamento de Caixa, Relatórios Livro Caixa
- **Rotinas em andamento (retomar):** Relatórios Saldo Contas Analítico — parou na pergunta de caminho de menu (item 3); faltam passo a passo completo, campos/parâmetros, erros comuns, rotinas relacionadas, módulos adicionais
- **Observações:**
  - Taxonomia de módulos foi bastante reestruturada antes da entrevista começar: removidos módulos duplicados/inexistentes (api, atsmais, dba, avulso, gadgets, web-cloud); movidos/renomeados vários sub-módulos; NFCe promovido a categoria própria com 4 sub-módulos.
  - Durante a entrevista de Windows » Caixa: 26 rotinas pré-mapeadas foram confirmadas como não pertencentes ao Caixa (23 mantidas em outros módulos, 3 apagadas por serem exclusivas); "Gestão de Centros de Custo" confirmada como inexistente em 5 módulos (confundida com "Cadastro Centro de Custo"); 8 rotinas identificadas como duplicatas do levantamento original (nomes "Movimentos X" ou variações repetindo rotinas já cadastradas) e mescladas/removidas, incluindo "Relatórios Fechamento de Caixas por Operador" (duplicata de "Relatórios Fechamento de Caixa").
  - "Cadastro de Usuários" confirmado pelo analista como existente em toda a família Windows (17 sub-módulos).
  - Windows » Business acumulou 23 rotinas confirmadas ao longo da entrevista (praticamente espelha as rotinas de Caixa).
  - "Fluxo de Caixa" foi corrigida: pré-mapeada em windows/caixa e windows/bancos, mas na verdade só existe no Business.
  - Rotinas que existem em 3+ módulos foram movidas para `wiki/rotinas/_compartilhadas/`.
  - Criados 3 procedimentos gerais reaproveitáveis: Busca Menu, padrão de botões/atalhos de cadastro, ressalva de que erros só ocorrem por problema pontual de versão.
