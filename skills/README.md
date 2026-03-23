# Skills

Skills são conjuntos de instruções ou código que ensinam um sistema a realizar uma tarefa específica. São mais simples que agentes — executam uma função bem definida sem tomar decisões complexas.

## Quando usar uma skill?

- Quando a tarefa é bem definida e repetível
- Para encapsular um processo que será reutilizado
- Quando não há necessidade de decisões autônomas

## Estrutura de uma skill

```
skills/
└── nome-da-skill/
    ├── README.md        <- descricao, uso, exemplos
    ├── SKILL.md         <- instrucoes para o agente usar a skill
    └── examples/        <- exemplos de entrada e saida
```

## Como adicionar uma nova skill

1. Crie uma branch: `git checkout -b feat/skill-nome`
2. Crie a pasta com `README.md` e `SKILL.md`
3. Documente com exemplos reais
4. Faça commit: `git commit -m "feat(skills): add nome-da-skill"`
5. Abra um Pull Request para `main`

## Skills disponíveis

| Nome | Descrição | Status |
|------|-----------|--------|
| *(vazio)* | *adicione suas skills aqui* | — |
