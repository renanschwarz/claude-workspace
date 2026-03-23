# Plugins

Plugins são extensões que adicionam capacidades a um sistema existente. Eles não agem sozinhos — precisam ser chamados por um agente ou sistema.

## Quando usar um plugin?

- Quando você quer estender o comportamento do Claude Code
- Para adicionar memória, acesso a ferramentas, integrações externas
- Quando a funcionalidade pode ser reutilizada em múltiplos contextos

## Estrutura de um plugin

```
plugins/
└── nome-do-plugin/
    ├── README.md        ← descrição, instalação, uso
    ├── index.ts         ← ponto de entrada e exports
    └── config.ts        ← configurações e defaults
```

## Como adicionar um novo plugin

1. Crie uma branch: `git checkout -b feat/plugin-nome`
2. Crie a pasta com os arquivos necessários
3. Documente no `README.md` (instalação + uso)
4. Faça commit: `git commit -m "feat(plugins): add nome-do-plugin"`
5. Abra um Pull Request para `main`

## Plugins disponíveis

| Nome | Descrição | Status |
|------|-----------|--------|
| claude-mem | Memória persistente entre sessões | ✅ Instalado |
