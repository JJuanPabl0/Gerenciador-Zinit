# *Zinit: Gerenciador de Plugins para Zsh*

### 1  O que é Zinit?

- O Zinit é um gerenciador de plugins e flexível para o shell Zsh. 
Ele permite que você *gerencie plugins, temas e scripts de forma eficiente, carregando-os rapidamente e otimizando a inicialização do terminal*. Com o Zinit, você pode personalizar e expandir as funcionalidades do Zsh de forma prática e organizada.

### 1.1 Caractériscas Principais:

- Carregamento assíncrono: Plugins são carregados em paralelo, melhorando o tempo de inicialização.

- Cache de plugins: Armazena os plugins já carregados, evitando downloads desnecessários.

- Suporte a plugins em diversas fontes: Você pode instalar plugins diretamente do GitHub, GitLab, Bitbucket, entre outros repositórios.

- Integração com outros gerenciadores de plugins: Zinit pode trabalhar com outros gerenciadores como o zplug, zgen, entre outros.

### 1.2 Como instalar o Zinit?

- Instalar via terminal: Cole esse comando no seu terminal para fazer a instalação do Zinit

        bash -c "$(curl -fsSL https://git.io/zinit-install)"

### 2 Adionando Plugins 

Após instalar o Zinit, abra as configurações do ZSH com o seguinte comando:
        
        nano ~/.zshrc

Caso esteja em duvida se instalou o zinit, digite o comando para analisar todos os seus arquivos inclundo os ocultos com detalhes sobre cada um, verifique se contém o item zenit:

        ls -la

