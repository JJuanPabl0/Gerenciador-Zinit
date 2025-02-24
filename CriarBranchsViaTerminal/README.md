## Criar uma Branch com README pelo Terminal


### 1. Crie o repositório no GitHub usando a API do GitHub

- Primeiro, você precisa autenticar-se na API do GitHub para criar o  repositório remotamente.

- Configure o token de autenticação do GitHub:

- Acesse [Configurações de Tokens Pessoais](https://github.com/settings/tokens) no GitHub.
Clique em "Generate new token (classic)", selecione permissões como repo, workflow, e admin:repo_hook. Copie o token gerado e salve em um local seguro

---
### 2. Configure o token no terminal: No zsh, execute:


        nano ~/.zshrc

Para abrir as configurações do .ZSH.

- Posteriormente, digite esse comando no final:

        export GITHUB_TOKEN=seu_token_aqui

Saia do terminal usando *Ctrl* + *S* (Para salvar) e *Ctrl* + *X* (Para sair).

- Use o seguinte comando para compilar e atualizar as alterações

        source ~/.zshrc

---
### 3. No terminal do ZSH, execute:

    curl -H "Authorization: token $GITHUB_TOKEN" \
     -d '{"name": "nome_do_repositorio", "private": false, "auto_init": true}' \
     https://api.github.com/user/repos


- Detalhes do comando:

"auto_init": true: Adiciona automaticamente um README.md no repositório recém-criado.

"private": false: Define o repositório como público. Mude para true se quiser que ele seja privado.

"name": "nome_do_repositorio": Substitua pelo nome desejado para o repositório.

---

### 4. Criação de Branch e Compilação

>Pausado, continuação em breve.