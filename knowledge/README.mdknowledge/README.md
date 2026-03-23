# Knowledge

Knowledge são bases de conhecimento e contextos que informam agentes e skills. Podem ser documentos, prompts de sistema, regras de negócio ou qualquer informação estruturada que oriente o comportamento da IA.

## Quando usar?

- Para guardar prompts de sistema reutilizáveis
- Regras de negócio ou contexto de projeto
- Documentação que o agente deve conhecer
- Exemplos de entrada/saída para orientar comportamento

## Estrutura

```
knowledge/
└── nome-do-contexto/
    ├── README.md        <- sobre esse conhecimento e como usar
    ├── system-prompt.md <- prompt de sistema (se aplicavel)
    └── examples/        <- exemplos de uso
```

## Como adicionar

1. Crie uma branch: `git checkout -b feat/knowledge-nome`
2. Crie a pasta com os arquivos
3. Faça commit: `git commit -m "feat(knowledge): add nome-do-contexto"`
4. Abra um Pull Request para `main`

## Bases disponíveis

| Nome | Descrição | Usado em |
|------|-----------|----------|
| *(vazio)* | *adicione suas bases aqui* | — |
