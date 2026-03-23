# Conventions

Guia de boas praticas para branches, commits e estrutura de pastas neste repositorio.

---

## Branches

Este repositorio segue o **GitHub Flow**. A branch `main` e sempre estavel.

### Nomenclatura

| Prefixo | Quando usar | Exemplo |
|---------|-------------|---------|
| `feat/` | Nova funcionalidade | `feat/plugin-memory` |
| `fix/` | Correcao de bug | `fix/agent-crash-on-start` |
| `docs/` | Somente documentacao | `docs/update-readme` |
| `chore/` | Manutencao e configs | `chore/update-deps` |
| `refactor/` | Reorganizacao sem mudar comportamento | `refactor/skill-loader` |

### Regras

- Nunca commite diretamente na `main`
- Use letras minusculas e hifens (sem underscores ou espacos)
- Seja especifico: `feat/skill-docx` e melhor que `feat/nova-skill`
- Delete a branch apos o merge

---

## Commits

Este repositorio usa o padrao **Conventional Commits**.

### Formato

```
tipo(escopo): descricao curta em minusculas
```

### Tipos validos

| Tipo | Quando usar |
|------|-------------|
| `feat` | Nova funcionalidade ou instalacao |
| `fix` | Correcao de bug |
| `docs` | Mudanca apenas em documentacao |
| `chore` | Tarefas de manutencao |
| `refactor` | Codigo reorganizado sem mudar comportamento |
| `test` | Adicao ou correcao de testes |

### Escopos comuns

`agents`, `plugins`, `skills`, `knowledge`, `docs`, `deps`

### Exemplos

```bash
feat(plugins): add claude-mem memory plugin
feat(skills): add docx generation skill
fix(agents): resolve crash on empty config
docs(readme): add installation instructions
chore(deps): update typescript to v5
refactor(plugins): extract loader to separate module
```

### Regras

- Use o imperativo: `add`, `fix`, `update` (nao `added` ou `adding`)
- Maximo de 72 caracteres na primeira linha
- Um commit = uma coisa. Nao misture instalacao com correcao
- Se precisar explicar mais, deixe uma linha em branco e escreva o corpo

---

## Estrutura de pastas

```
claude-workspace/
  agents/        <- agentes autonomos
  plugins/       <- extensoes de sistemas
  skills/        <- capacidades especificas
  knowledge/     <- bases de conhecimento
  docs/          <- documentacao geral
  README.md      <- visao geral do projeto
```

Cada item dentro dessas pastas deve ter seu proprio `README.md`.
