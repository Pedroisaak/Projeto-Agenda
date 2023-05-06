# Projeto Agenda

Um projeto agenda feito em node js utilizando como database o mongoDB em arquitetura MVC com o intuíto de aprender a programar em JS.


### Cadastro Usuario
<ul>
<li>Schema 'email' and 'password'
<li>Validação de email utilizando a biblioteca 'Validator' 
<li>Validação de e-mail já utilizado no cadastro por busca no database
<li>Validação do comprimento de caracteres de caracteres da senha
<li>Execução de mensagens com sucesso ou erro utilizando a biblioteca connect-flash
<li>Envio, em caso de sucesso, a senha formatada em hash para o servidor utilizando a biblioteca bcryptjs
</ul>

![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/101290219/170896496-7b999ab7-062a-4488-83f1-132ff8cbd012.gif)


### Login
<ul>
<li>Verifica no database se o usuário esta cadastrado
<li>Caso o login e senha correspondam, o usuário será logado e criará uma sessão usando a biblioteca express-session de 7 dias para o navegador
</ul>

### Home
<ul>
<li>Schema: 'titulo' and 'descricao"
<li>Boas-vindas ao usuário
<li>Libera o acesso de cadastro de usuários
<li>Renderiza pelo database,caso haja, os contatos já cadastrados pelo usuário
</ul>

### Cadastro Contato
<ul>
<li>Schema: 'nome', 'sobrenome', 'email' and 'senha'
<li>Validação para o envio do form, obrigatório o preenchimento do nome e email ou telefone
<li>Como feito no propósito de criar um CRUD, após inserir o usuário poderá edita-lo ou exclui-lo
</ul>

![ezgif com-gif-maker (4)](https://user-images.githubusercontent.com/101290219/170896616-74fe6ecb-adf2-4c47-a04a-73909910a9f4.gif)


### Segurança
<ul>
<li>Todo post gerará um toekn csrf utilizando a biblioteca csurf e validará com o token gerado no servidor afim de evitar ataques CSRF
<li>Utilizando a biblioteca helmet para evitar ataques tipicos do protocolo HTTP. 'Não é uma bala de prata mas ajuda'
</ul>

### Bibliotecas utilizadas no projeto
    "bcryptjs": "^2.4.3",
    "connect-flash": "^0.1.1",
    "connect-mongo": "^4.4.0",
    "core-js": "^3.9.1",
    "css-loader": "^5.1.3",
    "csurf": "^1.11.0",
    "dotenv": "^8.2.0",
    "ejs": "^3.1.6",
    "express": "^4.17.1",
    "express-session": "^1.17.1",
    "helmet": "^4.4.1",
    "mongoose": "^5.12.1",
    "regenerator-runtime": "^0.13.7",
    "style-loader": "^2.0.0",
    "validator": "^13.7.0"
    "@babel/cli": "^7.13.10",
    "@babel/core": "^7.13.10",
    "@babel/preset-env": "^7.13.10",
    "babel-loader": "^8.2.2",
    "nodemon": "^2.0.7",
    "webpack": "^5.27.0",
    "webpack-cli": "^4.5.0"



