Utilizacao de GIt

O Github constará nosso codigo branchs e todas features do projeto empregado para tal, abaixo veremos os principais comandos para se utilizar github.

- Primeiramente temos que ter instalado o git no nosso computador: [install git here](https://git-scm.com/downloads)
- Na raiz do nosso projeto vamos rodar o comando para inicializar um repositorio, inicialmente estara somente local em minha maquina.\
> git init
- Vamos criar na raiz de nosso projeto um arquivo chamado .gitignore este e para colocar pastas e arquivos que nao queremos que seja enviar ao github, por exemplos node_modules que e grande e nao tem essa necessidades, o arquivo ficara mais ou menos assim
> /node_modules
> /build
> /dist
> .DS_Store
> .env.local
> .env.development.local
> .env.test.local
> .env.production.local
> npm-debug.log*
> yarn-debug.log*
> yarn-error.log*
> yarn.lock
> package-lock.json

- Vamos ao github com nossa conta criada, criaremos um repositorio, o procedimento e bem simples e intuitivo, lembrando que o repositorio pode ser public ou privado.
- Ao criar o repos no mesmo tem um botao "code" nele podemos conectar via https ou ssl, vamos copiar o link https
- No cmd na raiz de nosso projeto vamos rodar um comando para adicionar a origin do repos onde linkara o repos local criado pelo git init ao repos criado no git
> git remote add origin https://github.com/repos/repos
- Tambem e necessario adicionar o proprietario do git email e nome de usuario, para isso rodaremos o comando
> git config --global user.email "user@mail.com"
> git config --global user.name "user099"
- O nosso ainda nao esta sincroniizado para isso vamos rodar um comando para que esse codigo fique em um stage area aguardando upload.
> git add .
- Vamos rodar um comando para adicionar um comentario aos arquivos do stage area que sera enviado ao github
> git commit -m "Meu comentario"
- Para enviar o codigo ao git digite o comando abaixo, apos sera necessario colocar email e senha do github para autenticar.
> git push origin master

Assim podemos ir no github e todo nosso codigo estara la, com facil acesso para pegar u compartilhar seja publico ou privado.

Agora para cada alteracao em nosso codigo assim que finalizarmos tal alteracao devemos commit nosso codigo no git
> git add .
> git commit -m "Meu comentario"
> git push origin master
* O master e a branch, no caso so tem uma branch temos que criar e sempre trabalhar em outra branch pois a master e somente producao

Apos finalizar um trabalho e commitar o codigo, finalizamos o dia, ao chegar para trabalhar novamente no projeto a primeira coisa a fazer e pegar os dados atualizados do guthub, rodando o comando:
> git pull origin nome_branch

Pois caso mais alguem esteja trabalhando no projeto pode ter codigo novo, entao deve se baixar o codigo novo para trabalhar em cima dele, e apos trabalhar e feito o commit, depois no git podemos gerir projeto fazer o merger, validar os commits ver as linhas que foram removidas ou incuidas no codigo e assim sucessivamente. 

#### Outros comandos git

- Criar uma branch nova
> git branch -b nome_branch
* observe que no seu cmd na frente do caminho da pasta fica informando qual branch vc esta e no vscode tbm, isso e importante para nao alterar codigo em lugar errado
- Mudar branch de trabalho
> git checkout nome_branch
* ira fazer um switch na branch no cmd, lembrando que o switch nao e feito se tiver arquivos sem commitar.
* Se voce tiver trabalhando em outra branch o comando para upload fica >git  push origin outra_branch<

---
Desenvolvido por: [Gil](https://github.com) | [Igor](https://github.com) | [Joilson](https://github.com)
