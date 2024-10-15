# Guia básico: GIT

# O que é o Git?

Git é um sistema de controle de versão distribuído amplamente utilizado no desenvolvimento de software. Ele permite que múltiplos desenvolvedores colaborem em um projeto, gerenciando alterações no código-fonte ao longo do tempo.

[Link da documentação oficial](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git)

## Por que o Git é usado?

- O Git rastreia as mudanças feitas em arquivos, permitindo que os desenvolvedores revisitem versões anteriores e entendam a evolução do código.
- Cada desenvolvedor tem uma cópia completa do repositório, incluindo seu histórico. Isso permite que os usuários trabalhem offline e façam alterações sem depender de um servidor central.
- Facilita a criação de ramos, permitindo que os desenvolvedores trabalhem em recursos ou correções isoladamente. Depois, esses ramos podem ser mesclados (merged) de volta ao ramo principal, geralmente chamado de `main` ou `master`.
- Alterações são registradas em "commits", que são como "marcadores" no tempo. Cada commit inclui um identificador único, uma mensagem descritiva e informações sobre as alterações feitas.
- Facilita a colaboração entre desenvolvedores, permitindo a criação de pull requests e revisões de código. Isso ajuda a garantir a qualidade do código antes que ele seja integrado ao projeto principal.
- Mantém um histórico completo das mudanças, permitindo que os desenvolvedores vejam quem fez o que e quando, o que é útil para auditorias e rastreamento de problemas.
- Frequentemente usado com plataformas de hospedagem de código, como GitHub, GitLab e Bitbucket, que oferecem interfaces gráficas e recursos adicionais para colaboração.

## Comandos do Git mais usados

Comandos essenciais que fornecem uma base sólida para trabalhar com o Git e realizar operações comuns em um repositório:

```bash
git init
git clone <url>
git status
git log
git add <arquivo>
git commit -m "mensagem"
git branch <nome da ramificação>
git checkout <nome da ramificação>
git merge <nome da ramificação>
git fetch
git pull
git push
git reset
git revert
git stash
git stash pop 
```
## Instalando o GIT:

Para começar a utilizar o Git é necessário realizar a instalação
 No linux: 
 ```bash
 $ sudo apt-get install git-all
```
[Para Windows baixe aqui](http://git-scm.com/download/win)

## Configurando o Git
Depois de instalar o Git é necessário fazer a configuração.
Com seu nome de usuário e email, cada commit usa essa informação para identificar seus commits de forma imutável
 ```bash
 $ git config --global user.name "Fulano de Tal"
```
 ```bash
 $ git config --global user.email fulanodetal@exemplo.br
```

## Iniciando um repositório

Para iniciar o versionamento de um projeto local usando os comandos Git, acesse a pasta do repositório e no terminal execute o comando: Git init: Inicializa um novo repositório Git vazio 
```bash
 $ git init
```

## Adicionando as alterações
Para que o Git adicione o arquivo no versionamento:

Git add <arquivo>: Adiciona um ou mais arquivos ao índice para serem incluídos no próximo commit. Você pode usar “$ git add .” para adicionar todos os arquivos alterados.
```bash
 $ git add .
```
E para realizar o commit:

Git commit -m "mensagem": Cria um novo commit com as alterações adicionadas, incluindo uma mensagem descritiva.
  ```bash
 $ git commit -m "Texto do commit"
```
  
## Criando uma branch
Para criarmos uma nova branch a partir da master:

Git branch <nome-da-ramificação>: Cria uma nova ramificação.
E o git branch lista todas as ramificações no repositório.

## Adicionando ao um repositório remoto
Adicionando o arquivo a um repositório remoto, aqui para o exemplo, o GitHub:

Git remote add origin <url>: Adiciona as alteraçẽos a um repositório remoto.
E para o Git log: Exibe o histórico de commits no repositório.
  ```bash
 $ git log
```
##  Enviando as alterações para o GitHub
Enviando as alterações para o repositório remoto
Git push: Envia as alterações locais para o repositório remoto.
```bash
 $ git push
```
## Link dos nossos repositórios:
  
SIS-SURFACE:  
[Link do repositório](https://source.cloud.google.com/sis-surface?authuser=0)
  
SPARK-EYES:  
[Link do repositório](https://source.cloud.google.com/spark-eyes?authuser=0)
  
SMART-DIE:  
[Link do repositório](https://source.cloud.google.com/smart-die?authuser=0)