# claude-workspace

Workspace para instalar e gerenciar agentes, plugins, skills e bases de conhecimento com boas praticas de Git.

---

## Estrutura

| Pasta | O que vai aqui |
|-------|----------------|
| [agents/](./agents/) | Agentes autonomos que executam tarefas complexas |
| [plugins/](./plugins/) | Extensoes que adicionam capacidades a sistemas |
| [skills/](./skills/) | Instrucoes para tarefas especificas e repetíveis |
| [knowledge/](./knowledge/) | Bases de conhecimento, prompts e contextos |
| [docs/](./docs/) | Documentacao geral do projeto |

---

## Primeiros passos

- [Getting Started](./docs/getting-started.md)
- [Convencoes de branches e commits](./docs/conventions.md)

---

## Fluxo rapido

```bash
git clone https://github.com/renanschwarz/claude-workspace.git
git checkout -b feat/plugin-nome
git commit -m "feat(plugins): add nome-do-plugin"
```

---

## Plugins instalados

| Nome | Descricao | Repositorio |
|------|-----------|-------------|
| claude-mem | Memoria persistente entre sessoes | [claudecode](https://github.com/renanschwarz/claudecode) |
docs(docs): add getting started guide
