# ATS Informática — Coleta de Conhecimento com Analista (Entrevista)

## 1. O que é esta pasta

Esta é uma wiki de trabalho para **entrevistar um analista** e registrar, em pt-BR, o que são e como usar os módulos e rotinas do sistema ATS. O conteúdo já vem **pré-mapeado** (nomes de módulos e rotinas levantados anteriormente), mas **sem conteúdo real** — cada rotina é um esqueleto aguardando a entrevista.

Você (Claude) conduz a entrevista com o analista, uma pergunta de cada vez, e vai salvando as respostas diretamente nos arquivos `.md` desta wiki, marcando o progresso nos arquivos de controle. Ao final, esta pasta será enviada de volta para mesclar na wiki principal do projeto.

**Todo conteúdo é escrito em português do Brasil (pt-BR).** Nomes de pasta, chaves YAML e identificadores de código continuam em inglês.

---

## 2. Regra de ouro: ordem da entrevista

**Nunca entreviste uma rotina de um módulo que ainda não foi confirmado.**

A ordem obrigatória é:

1. **Confirmar módulos** (`wiki/_controle/controle-modulos.md`) — antes de qualquer coisa, percorra a lista de módulos pré-mapeados com o analista. Para cada um, pergunte: *"O módulo [nome] existe hoje no sistema? Ainda é usado com esse nome?"*
   - Se sim → marque `[x]` em `controle-modulos.md`.
   - Se não existe mais / foi renomeado / nunca existiu → marque `[-]` e anote o motivo ao lado (ex: `[-] Windows » Self Color — descontinuado em 2024, confirmado com analista`).
   - Se o analista mencionar um módulo que não está na lista → adicione uma nova linha em `controle-modulos.md` E crie o arquivo correspondente em `wiki/modulos/`.
2. **Só depois de um módulo estar confirmado `[x]`**, avance para as rotinas daquele módulo em `wiki/_controle/controle-rotinas.md`.
3. Para cada módulo confirmado, **mostre a lista de rotinas pré-mapeadas daquele módulo** e pergunte ao analista: *"Essas são as rotinas de [módulo] hoje? Alguma não existe mais? Falta alguma?"*
   - Rotina confirmada → prossiga para entrevista de conteúdo (Seção 3).
   - Rotina que não existe mais → marque com `[-]` em `controle-rotinas.md`, não crie conteúdo, adicione nota.
   - Rotina nova mencionada pelo analista → crie novo arquivo em `wiki/rotinas/` seguindo o Schema (Seção 5) e adicione linha em `controle-rotinas.md`.
4. Trabalhe **um módulo por vez, até esgotar todas as rotinas confirmadas daquele módulo**, antes de passar ao próximo módulo — não pule entre módulos no meio do processo, para não perder o fio da meada com o analista.

---

## 3. Entrevistando uma rotina (perguntas obrigatórias)

Para cada rotina, pergunte — **não pressuponha respostas**, e não avance para a próxima pergunta até ter uma resposta utilizável (pode ser "não sei" / "não se aplica", tudo bem, registre):

1. **O que é / pra que serve** essa rotina, em 1-2 frases simples?
2. **Quem usa** (perfil de usuário: operador de caixa, financeiro, admin, etc.)?
3. **Como usar — passo a passo.** Peça o caminho de menu/tela e a sequência de ações.
4. **Campos e parâmetros importantes** — existe algo que o usuário costuma errar ou não entender?
5. **Erros comuns** — quais problemas costumam aparecer ao usar essa rotina? (Se envolver banco de dados, SQL, Firebird, registro do Windows, ou operação de servidor, classifique a página como `audience: analyst` — ver Seção 6.)
6. **Rotinas relacionadas** — SEMPRE pergunte: *"Essa rotina se relaciona com quais outras rotinas? Ela depende de alguma outra rodar antes? Alguma rotina é chamada a partir dela?"* Isso é essencial para montar o grafo de relacionamento no Obsidian — não pule esta pergunta.
7. **Outros módulos** — SEMPRE pergunte: *"Essa rotina também existe ou é usada em outro módulo além de [módulo atual]?"* Se sim, adicione o módulo à lista `modulos:` do frontmatter E confirme se esse outro módulo já está na lista de `controle-modulos.md` (senão, adicione).

Depois de coletar as respostas:
- Preencha o corpo do arquivo `wiki/rotinas/<slug>.md` substituindo os placeholders `_(a preencher...)_`.
- Preencha `relations:` no frontmatter com as relações citadas (formato: `- from: "Nome da Rotina" \n  type: RELACIONA_COM|DEPENDE_DE|CHAMA \n  to: "Outra Rotina"`).
- Use `[[rotinas/outra-rotina|Nome da Outra Rotina]]` no corpo do texto para linkar (sintaxe Obsidian).
- Atualize `status_entrevista: concluida` e `data_atualizacao` no frontmatter.
- Marque `[x]` na linha correspondente em `wiki/_controle/controle-rotinas.md`.
- Se **todas** as rotinas de um módulo estiverem `[x]`, volte em `controle-modulos.md` e acrescente uma nota "— rotinas concluídas" (não crie novo campo, apenas comente ao lado do `[x]` já marcado).

Se a entrevista for pausada no meio de uma rotina (analista precisa parar), salve o que já foi coletado no arquivo com `status_entrevista: em-andamento` e registre em `wiki/log.md` o ponto exato onde parou, para retomar depois.

---

## 4. O grafo de relacionamento (essencial)

O objetivo final é ter um grafo claro e navegável no Obsidian: quais rotinas pertencem a quais módulos, e quais rotinas se relacionam entre si. Para isso:

- Toda rotina **deve** ter pelo menos um módulo em `modulos:` no frontmatter (nunca deixe vazio depois de entrevistada).
- Toda relação entre rotinas mencionada pelo analista **deve** virar um wikilink `[[...]]` no corpo do texto E uma entrada em `relations:` no frontmatter.
- Se uma rotina existe em 2+ módulos, ela continua sendo um único arquivo em `wiki/rotinas/` (não duplique) — apenas liste todos os módulos em `modulos:` e descreva as diferenças de comportamento por módulo dentro do próprio arquivo, se houver (mesmo padrão de "rotinas compartilhadas" da wiki principal — ver `wiki/rotinas/_compartilhadas/`).
- Depois de confirmado um módulo, gere/atualize o arquivo `wiki/modulos/<slug>.md` com a lista real de rotinas (a lista pré-carregada é só um ponto de partida).

---

## 5. Schema de Frontmatter

Idêntico ao da wiki principal, com um campo extra de controle da entrevista:

```yaml
---
id: PREFIX-slug-da-pagina   # ROT- para rotina, MOD- para modulo
title: "Título em pt-BR"
type: rotina | modulo
audience: all | analyst | a-definir   # 'a-definir' até a entrevista definir (ver Seção 6)
modulos: []                # slugs de wiki/modulos/, ex: ["windows/caixa"]
tags: []
status: active | draft     # 'active' só quando o conteúdo real foi preenchido
status_entrevista: pendente | em-andamento | concluida | nao-existe
data_criacao: YYYY-MM-DD
data_atualizacao: YYYY-MM-DD
fontes: []                 # deixe vazio — não há raw/ nesta pasta, a fonte é a entrevista
entities: []
relations:
  - from: Entidade A
    type: RELACIONA_COM | DEPENDE_DE | CHAMA
    to: Entidade B
---
```

Quando uma rotina/módulo é confirmada com conteúdo real, mude `status: draft` → `status: active` E `status_entrevista: pendente` → `concluida` ao mesmo tempo.

---

## 6. Classificação de audiência (`audience`)

Mesma regra da wiki principal — aplique durante a entrevista, não deixe `a-definir` na versão final:

> [!IMPORTANT] Regra absoluta sobre banco de dados
> Se a rotina envolve SQL, Firebird (gfix, gbak, isql, SYSDBA, RDB$, .fdb), edição de tabela, backup/restore de banco, registro do Windows, arquivos .ini/.cfg, operação de servidor, ou erro crítico de sistema (corrupção de dados, deadlock, crash) — é **obrigatoriamente `audience: analyst`**, sem exceção.

Caso contrário (uso normal, erros de rejeição fiscal NF-e/NFC-e, FAQ) → `audience: all`.

---

## 7. Estrutura desta pasta

```
CLAUDE.md                       este arquivo
README.md                       instruções rápidas para o analista (não técnico)
.claude/skills/entrevista-rotinas/SKILL.md    skill que conduz a entrevista (/entrevista-rotinas)
wiki/
  _controle/
    controle-modulos.md         checklist de confirmação de módulos (fazer PRIMEIRO)
    controle-rotinas.md         checklist de entrevista de rotinas, agrupado por módulo
  modulos/                      páginas de módulo (esqueleto pré-carregado)
  rotinas/                      páginas de rotina (esqueleto pré-carregado, 1549 arquivos)
  rotinas/_compartilhadas/      rotinas que pertencem a 3+ módulos (mover para cá quando identificado)
  troubleshooting/ erros/ procedimentos/ faq/   crie aqui se a entrevista revelar esse tipo de conteúdo
  outputs/                      não usado nesta pasta
  log.md                        registro de cada sessão de entrevista (criar no primeiro uso)
  index.md                      catálogo — atualize ao final de cada sessão
```

---

## 8. Log de sessão

Ao final de cada sessão de entrevista (ou quando o analista pedir para parar), acrescente em `wiki/log.md`:

```markdown
## [YYYY-MM-DD] entrevista | Módulo X
- **Módulos confirmados nesta sessão:** lista
- **Rotinas concluídas:** N
- **Rotinas em andamento (retomar):** nome — ponto onde parou
- **Observações:** decisões do analista, módulos descontinuados, etc.
```

---

## 9. Comando para começar

O analista deve abrir esta pasta no Claude Code e digitar `/entrevista-rotinas` (ou simplesmente "vamos começar"). A skill em `.claude/skills/entrevista-rotinas/SKILL.md` assume a condução a partir daí.
