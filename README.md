# Guia de Conventional Commits

Este repositório contém um guia de boas práticas para escrever mensagens de commit seguindo a convenção [Conventional Commits](https://www.conventionalcommits.org/).

## Tipos de commits

- **build**: Mudanças que afetam o sistema de build ou dependências externas (escopos: gradle, gulp, npm, webpack)
    - Exemplo: `build: configurar webpack para produção`
- **ci**: Mudanças em arquivos de configuração e scripts de CI (escopos: travis, circle, gitlab-ci)
    - Exemplo: `ci: adicionar configuração de deploy no Travis CI`
- **chore**: Mudanças na configuração do build ou em ferramentas auxiliares e bibliotecas, como a geração de documentação.
    - Exemplo: `chore: atualizar dependências do projeto`
- **docs**: Apenas mudanças na documentação
    - Exemplo: `docs: atualizar README com novas instruções de setup`
- **feat**: Uma nova funcionalidade para o usuário.
    - Exemplo: `feat: adicionar validação para o campo de email`
- **fix**: Correção de bugs
    - Exemplo: `fix: corrigir erro de digitação no título da página`
- **perf**: Mudança de código que melhora o desempenho
    - Exemplo: `perf: otimizar consulta SQL`
- **refactor**: Mudança de código que não corrige um bug nem adiciona uma funcionalidade
    - Exemplo: `refactor: renomear variáveis para melhorar legibilidade`
- **revert**: Reverter para um commit anterior
    - Exemplo: `revert: reverter commit 1234abcd`
- **style**: Mudanças que não afetam o significado do código (espaço em branco, formatação, ponto e vírgula ausente, etc)
    - Exemplo: `style: remover espaços em branco`
- **test**: Adicionando ou corrigindo testes existentes
    - Exemplo: `test: adicionar testes unitários para a função de login`


## Estrutura de uma mensagem de commit

```
<tipo>(<escopo opcional>): <descrição curta>

[corpo opcional]

[rodapé opcional]
```

### Exemplo

```
feat(auth): adicionar suporte para autenticação OAuth

Adiciona suporte para autenticação via OAuth com provedores externos.
Essa funcionalidade inclui:
- Login com Google
- Login com Facebook

BREAKING CHANGE: A função de login agora requer uma configuração de provedores.
```

### Exemplos Práticos

- **Adicionar nova funcionalidade**
    ```
    feat: adicionar suporte para autenticação OAuth
    ```
- **Corrigir bug**
    ```
    fix: corrigir erro de digitação no título da página
    ```
- **Melhorar desempenho**
    ```
    perf: otimizar consulta SQL
    ```
- **Refatorar código**
    ```
    refactor: renomear variáveis para melhorar legibilidade
    ```
- **Reverter commit anterior**
    ```
    revert: reverter commit 7a55c6c
    ```
- **Adicionar testes**
    ```
    test: adicionar testes unitários para a função de login
    ```
- **Atualizar documentação**
    ```
    docs: atualizar README com novas instruções de setup
    ```
- **Atualizar dependências**
    ```
    chore: atualizar dependências do projeto
    ```
- **Configurar CI/CD**
    ```
    ci: adicionar configuração de deploy no Travis CI
    ```
- **Configurar build**
    ```
    build: configurar webpack para produção
    ```
- **Corrigir estilo**
    ```
    style: remover espaços em branco
    ```

