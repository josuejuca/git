### Manual de Comandos Git

#### Introdução

O Git é um sistema de controle de versão distribuído que permite aos desenvolvedores rastrear alterações no código-fonte durante o desenvolvimento de software. Criado por Linus Torvalds em 2005, o Git facilita a colaboração em projetos de software, permitindo que múltiplos desenvolvedores trabalhem em diferentes partes de um projeto ao mesmo tempo. Este manual apresenta uma visão geral dos principais comandos do Git, ajudando você a iniciar e gerenciar seu repositório de código de maneira eficaz.

#### Configuração Inicial

Antes de começar a usar o Git, é necessário configurar algumas informações básicas, como seu nome de usuário e e-mail. Essas informações serão usadas para associar seus commits a você.

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
```

#### Repositório

Para começar a usar o Git, você precisa inicializar um novo repositório ou clonar um repositório existente.

- **Inicializar um novo repositório**:
  ```bash
  git init
  ```

- **Clonar um repositório existente**:
  ```bash
  git clone https://github.com/usuario/repositorio.git
  ```

#### Controle de Versão Básico

Os comandos a seguir ajudam a adicionar, confirmar e visualizar alterações no seu repositório.

- **Adicionar arquivos ao índice (staging area)**:
  ```bash
  git add arquivo.txt
  git add .
  ```

- **Confirmar as alterações adicionadas ao índice**:
  ```bash
  git commit -m "Mensagem de commit"
  ```

- **Exibir o status das alterações no repositório**:
  ```bash
  git status
  ```

- **Mostrar o histórico de commits**:
  ```bash
  git log
  ```

#### Branches

Branches são usadas para desenvolver funcionalidades isoladas umas das outras. O Git permite criar, listar e excluir branches com facilidade.

- **Listar, criar ou excluir branches**:
  ```bash
  git branch
  git branch nova-branch
  git branch -d branch-antiga
  ```

- **Mudar para outra branch ou restaurar arquivos da árvore de trabalho**:
  ```bash
  git checkout nome-da-branch
  git checkout -b nova-branch
  ```

#### Mesclagem e Rebase

Mesclar e fazer rebase são formas de integrar alterações de diferentes branches.

- **Mesclar uma branch na branch atual**:
  ```bash
  git merge nome-da-branch
  ```

- **Reaplicar commits da branch atual em cima de outra base**:
  ```bash
  git rebase nome-da-branch
  ```

#### Sincronização com Repositórios Remotos

Para colaborar com outros desenvolvedores, é importante saber como trabalhar com repositórios remotos.

- **Gerenciar conexões com repositórios remotos**:
  ```bash
  git remote add origin https://github.com/usuario/repositorio.git
  ```

- **Buscar alterações do repositório remoto sem integrá-las**:
  ```bash
  git fetch origin
  ```

- **Atualizar o repositório local com as mudanças do repositório remoto e mesclá-las**:
  ```bash
  git pull origin master
  ```

- **Enviar as alterações para o repositório remoto**:
  ```bash
  git push origin master
  ```

#### Desfazendo Alterações

O Git também permite desfazer alterações de várias formas, seja resetando o índice ou criando commits de reversão.

- **Resetar o índice e/ou o diretório de trabalho para um estado anterior**:
  ```bash
  git reset --soft HEAD~1
  git reset --hard HEAD~1
  ```

- **Criar um novo commit que desfaz as alterações de um commit anterior**:
  ```bash
  git revert <commit>
  ```

#### Outros Comandos Úteis

Alguns comandos adicionais do Git são úteis para gerenciar suas alterações e marcar pontos importantes na história do repositório.

- **Armazenar temporariamente as mudanças de trabalho não confirmadas**:
  ```bash
  git stash
  git stash apply
  ```

- **Marcar um ponto específico na história do repositório como importante**:
  ```bash
  git tag -a v1.0 -m "Versão 1.0"
  ```

Esses são alguns dos comandos básicos e mais utilizados do Git. Com este manual, você pode gerenciar seu repositório de código e colaborar com outros desenvolvedores de forma eficaz. Se precisar de mais detalhes sobre algum comando específico ou sobre outros comandos, sinta-se à vontade para perguntar no email: etc.juca@gmail.com
