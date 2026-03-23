# Getting Started

Bem-vindo ao claude-workspace! Este guia explica como configurar o ambiente e comecar a contribuir.

---

## Pre-requisitos

- Git instalado
- Node.js 18+
- Conta no GitHub

---

## 1. Clonar o repositorio

```bash
git clone https://github.com/renanschwarz/claude-workspace.git
cd claude-workspace
```

---

## 2. Estrutura do projeto

```
claude-workspace/
  agents/        <- agentes autonomos
  plugins/       <- extensoes (ex: claude-mem)
  skills/        <- capacidades especificas
  knowledge/     <- bases de conhecimento
  docs/          <- documentacao
  README.md
```

Cada pasta tem seu proprio README explicando o que vai ali.

---

## 3. Fluxo de trabalho

Sempre siga este fluxo ao adicionar algo novo:

```bash
# 1. Garanta que a main esta atualizada
git checkout main
git pull

# 2. Crie uma branch com nome descritivo
git checkout -b feat/plugin-nome

# 3. Faca suas alteracoes...

# 4. Commit com mensagem padrao
git add .
git commit -m "feat(plugins): add nome-do-plugin"

# 5. Envie a branch
git push origin feat/plugin-nome

# 6. Abra um Pull Request no GitHub
# 7. Apos merge, delete a branch
```

---

## 4. Convencoes

Leia o guia completo de convencoes antes de contribuir:

- [Convencoes de branches e commits](./conventions.md)

---

## 5. Adicionando um novo item

| O que adicionar | Pasta destino | Prefixo do commit |
|----------------|--------------|-------------------|
| Agente | `agents/` | `feat(agents):` |
| Plugin | `plugins/` | `feat(plugins):` |
| Skill | `skills/` | `feat(skills):` |
| Conhecimento | `knowledge/` | `feat(knowledge):` |

Cada item novo deve ter sua propria pasta com um `README.md` descrevendo o que faz e como usar.
