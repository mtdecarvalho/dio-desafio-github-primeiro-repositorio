# Desafio de Projeto sobre Git/GitHub da DIO

Repositório criado para o Desafio de Projeto, que consiste na criação de um repositório com anotações sobre o funcionamento de Git e GitHub.

## Passo a passo para a criação de um repositório local e sua sincronização com um repositório remoto

Para criar um repositório, primeiro devemos utilizar algum terminal que aceite comandos do git. Muitos usam o Git Bash, que já vem com o próprio Git. Eu prefiro utilizar os comandos do git integrados diretamente no Powershell do Windows ou no Bash do Linux.

Qualquer que seja sua preferência, o comando para inicializar um repositório local é:

```
git init
```

Para confirmar se o repositório foi realmente criado ou não, podemos usar o comando:

```
git status
```

Que nos informará o estado e informações do repositório no local, como o nome da branch atual.

Feito isso, você agora tem um repositório git local no seu computador. Porém, isso só inicializa um repositório, e não adiciona nada no mesmo.

Para adicionar arquivos em seu repositório, é necessário adicioná-los ao próximo commit e confirmar o commit. Para adicionar os arquivos ao commit, usamos:

```
git add caminho_ou_nome_do_arquivo
```

Esse comando adicionará o(s) arquivo(s) especificado(s) ao commit.

Para ver quais arquivos estão separados para o próximo commit, podemos usar novamente o comando:

```
git status
```

Que, dessa vez, informará sobre os arquivos que estão separados para o commit.

Agora, você precisar confirmar o commit dessa alteração no repositório. Para isso, utilize o comando:

```
git commit -m "Mensagem do commit"
```

Todo commit **precisa** de uma mensagem. Tente ser detalhado quanto ao que exatamente está incluído no commit, como quais arquivos foram adicionados, quais foram alterados e quais foram removidos.

Agora, vamos criar uma branch. Para isso, use esse comando:

```
git branch -M nome_da_branch
```

Feito tudo isso, agora você precisa sincronizar esse repositório local com algum repositório remoto. Para isso, será necessário criar um repositório no GitHub (ou algum site equivalente, porém essas anotações servem apenas para o GitHub).

Para criar um repositório no GitHub, entre com sua conta e clique em New, como na imagem abaixo:

![Criar novo repositório](https://i.imgur.com/DCvaHJ0.png)

Que te levará para a seguinte tela:

![Tela de criação de repositório](https://i.imgur.com/WC9fT7W.png)

Aqui, podemos escolher o nome do repositório, uma descrição opcional, sua visibilidade e algumas opções, como a criação de um arquivo README (como esse que você está lendo agora), de um .gitignore e até mesmo uma licença para seu repositório.

Após escolher como você quer o seu repositório com as mesmas opções do que eu fiz acima, chegará enfim a esta tela:

![Tela final de criação de repositório](https://i.imgur.com/Vdga0Uj.png)

Aqui temos um tutorial do próprio GitHub para adicionar arquivos no GitHub, que talvez seja do seu interesse ler. Mas o que importa para nós é o link informado logo ali em cima, dentro da janela que diz Quick setup. Esse é o link do seu repositório git remoto. Para adicioná-lo ao seu repositório local, rode o seguinte comando:

```
git remote add origin link_para_o_repositorio_do_github
```

O link informado pode ser HTTPS ou SSH. Escolha de acordo com sua preferência.

Finalmente, vamos dar um push (empurrar) essas alterações para o nosso repositório remoto, com o seguinte comando:

```
git push -u origin nome_da_branch
```

Note que o nome da branch neste comando tem que ser o **mesmo nome da branch criada anteriormente.**

Atualizando o repositório, temos a confirmação de que nossos repositórios remotos e locais estão sincronizados, como na foto abaixo:

![Tela do repositório sincronizado](https://i.imgur.com/YYWeHu8.png)

Isso conclui essas anotações. Espero que as mesmas estejam claras, já que é a primeira vez que disponibilizo um "tutorial" assim aqui no GitHub.


## Links úteis:

- [Download do Git](https://git-scm.com/downloads)
- [Sintaxe básica de Markdown](https://www.markdownguide.org/basic-syntax/)
- [Repositório criado durante o tutorial](https://github.com/mtdecarvalho/repo-teste)