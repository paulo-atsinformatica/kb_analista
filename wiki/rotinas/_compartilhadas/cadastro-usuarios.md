---
id: ROT-cadastro-usuarios
title: "Cadastro de Usuários"
type: rotina
audience: all
modulos: ["windows/caixa", "windows/faturamento", "windows/contas-a-pagar", "windows/contas-a-receber", "windows/bancos", "windows/livros-fiscais", "windows/sped", "windows/compras", "windows/os", "windows/materiais", "windows/business", "windows/resulth-emissor-nfe", "windows/sintegra-cs", "windows/entregas-cs", "windows/retaguarda-ecf", "windows/backupnow", "windows/resulth-offline"]
tags: []
status: active
status_entrevista: concluida
data_criacao: 2026-07-16
data_atualizacao: 2026-07-16
fontes: []
entities: []
relations:
  - from: Cadastro de Usuários
    type: RELACIONA_COM
    to: Cadastro de Operadores de Caixa
  - from: Cadastro de Usuários
    type: RELACIONA_COM
    to: Abertura de Caixa
---

## Visão Geral
Rotina usada para cadastrar os usuários que podem acessar os sistemas da ATS. É por meio dela que se libera o acesso a todas as rotinas do sistema, cadastrando os usuários de acordo com a função que exercem na empresa. É uma rotina comum a toda a família Windows (existe em todos os sub-módulos Windows).

## Quem Usa
Deve ser feito diretamente por um responsável da empresa — não deve ser liberado para todos os usuários acessarem.

## Módulos onde esta rotina existe
Existe em todos os sub-módulos da família Windows: Caixa, Faturamento, Pagar, Receber, Bancos, Livros, Sped, Compras, Ordem de Serviço, Materias, Business, ResulthEmissorNFe, SintegraCs, EntregasCs, RetaguardaECF, BackupNow, Resulth Offline.

## Como Usar (passo a passo)
1. Acessar **Cadastros » Usuários**, ou usar o Busca Menu.
2. Ver o [[procedimentos/padrao-botoes-cadastro|padrão de botões e atalhos de cadastro]] (Inclusão, Alteração, Exclusão, Consulta, Lista, Pesquisa).
3. Informar o nome do usuário, depois a senha (aperta Enter para informar a senha novamente, como confirmação).
4. Marcar o campo **Ativo**.
5. Preencher os demais campos, que são as permissões de acesso do usuário, de acordo com sua função na empresa (Gerente, Vendedor, etc.).

## Campos e Parâmetros Importantes
- Sequência: Nome → Senha (confirmada com Enter) → campo Ativo.
- O campo **Ativo** precisa estar marcado, senão o usuário não consegue acessar o sistema.
- Os demais campos são permissões de acesso, preenchidas de acordo com a função do usuário.
- O campo **É Gerente** concede permissões diferenciadas, como liberação de desconto, entre outras funções.

## Erros Comuns / Pontos de Atenção
- Esquecer de marcar o campo Ativo após o cadastro — o usuário não consegue acessar o sistema.
- Ao desligar um funcionário que já tenha feito lançamentos no sistema, apenas **desmarcar o Ativo** — nunca excluir o usuário, para manter o histórico de lançamentos e ao mesmo tempo impedir o acesso.

## Rotinas Relacionadas
- [[rotinas/cadastro-operadores|Cadastro de Operadores de Caixa]] — cada operador precisa estar vinculado a um usuário (relação 1 para 1).
- [[rotinas/abertura-de-caixa|Abertura de Caixa]] — o usuário é informado na abertura de caixa.
