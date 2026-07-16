---
name: entrevista-rotinas
description: Conduz a entrevista estruturada com o analista para coletar conhecimento sobre módulos e rotinas do sistema ATS, salvando o progresso na wiki e nos arquivos de controle. Use quando o analista disser "vamos começar", "continuar entrevista", "/entrevista-rotinas" ou similar.
---

# Skill: Entrevista de Rotinas

Você conduz uma entrevista em pt-BR com um analista da ATS Informática para preencher o conteúdo real de módulos e rotinas do sistema. As regras completas de schema, classificação de audiência e formato de arquivo estão em `CLAUDE.md` na raiz desta pasta — **leia esse arquivo antes de começar, se ainda não leu nesta sessão.**

## Passo a passo ao ser acionada

### 1. Verificar estado atual
Leia `wiki/_controle/controle-modulos.md` e `wiki/_controle/controle-rotinas.md`.

- Se há módulos ainda sem `[x]` ou `[-]` → vá para o Passo 2 (confirmação de módulos).
- Se todos os módulos já estão confirmados, mas há rotinas `[ ]` em módulos já `[x]` → vá direto para o Passo 3 (entrevista de rotina) no primeiro módulo com pendências.
- Se tudo está `[x]` → informe ao analista que a coleta está completa e pergunte se quer revisar algo.

### 2. Confirmação de módulos (uma vez, no início)
Apresente a lista de módulos pré-mapeados **em grupos pequenos** (ex: por seção — Windows, Web, Gadgets, Mobile, etc.), não os 77 de uma vez. Para cada grupo, pergunte quais existem, quais foram descontinuados, e se falta algum módulo novo. Vá atualizando `controle-modulos.md` em tempo real conforme as respostas chegam — não espere confirmar tudo para começar a salvar.

Quando o analista mencionar um módulo novo (fora da lista pré-carregada):
- Crie `wiki/modulos/<slug-novo>.md` seguindo o mesmo template dos módulos existentes nessa pasta.
- Acrescente uma linha em `controle-modulos.md` na seção apropriada.

### 3. Entrevista de rotinas, módulo por módulo
Pegue o **primeiro módulo confirmado `[x]`** que ainda tem rotinas pendentes em `controle-rotinas.md`. Diga ao analista qual módulo vocês vão tratar agora e quantas rotinas estão pré-mapeadas para ele.

Mostre a lista de rotinas pré-mapeadas daquele módulo (nomes apenas, não o conteúdo) e pergunte: quais existem, quais não existem mais, falta alguma. Ajuste `controle-rotinas.md` e crie arquivos novos se necessário.

Depois, entreviste **uma rotina de cada vez**, na ordem da lista, seguindo exatamente as 7 perguntas da Seção 3 do `CLAUDE.md`. Não pule a pergunta de relacionamento (item 6) nem a de módulos adicionais (item 7) — são a base do grafo.

Após cada rotina:
1. Escreva o conteúdo no arquivo `wiki/rotinas/<slug>.md` correspondente.
2. Atualize frontmatter (`status`, `status_entrevista`, `audience`, `modulos`, `relations`, `data_atualizacao`).
3. Marque `[x]` em `controle-rotinas.md`.
4. Confirme rapidamente com o analista antes de seguir para a próxima ("Ok, registrado. Próxima: [nome]?").

Quando todas as rotinas de um módulo estiverem `[x]`, atualize `wiki/modulos/<slug>.md` com a lista final real de rotinas e avise o analista que o módulo está completo, perguntando se quer seguir para o próximo.

### 4. Encerrando a sessão
Quando o analista disser que precisa parar (ou você perceber sinais de encerramento — "por hoje é só", "depois continuamos"):
1. Garanta que a rotina em andamento está salva com `status_entrevista: em-andamento` se incompleta, ou `concluida` se terminou.
2. Acrescente uma entrada em `wiki/log.md` conforme o formato da Seção 8 do `CLAUDE.md`.
3. Resuma em 3-5 linhas o que foi feito na sessão e o que falta.
4. Informe que o analista pode retomar depois digitando `/entrevista-rotinas` de novo — a skill vai reler os arquivos de controle e continuar do ponto certo.

### 5. Atualizar index.md periodicamente
A cada módulo inteiro concluído, atualize `wiki/index.md` (crie se não existir, mesmo formato da wiki principal — tabela por tipo de página) com as rotinas e módulos já `active`.

## Princípios gerais
- Pergunta por vez — não jogue uma lista de 7 perguntas de uma vez no analista.
- Sempre em pt-BR.
- Não invente conteúdo — se o analista não souber, registre "a confirmar depois" no corpo do texto e mantenha `status_entrevista: em-andamento`.
- Nunca marque `[x]` em `controle-rotinas.md` sem o conteúdo estar de fato escrito no arquivo.
- Se o analista corrigir um módulo de uma rotina no meio da entrevista, atualize `modulos:` no frontmatter e mova/atualize as referências em `controle-rotinas.md` de ambos os módulos envolvidos.
