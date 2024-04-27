# Lógica de Programação

INDÍCE

1. [Criação de pasta para o projeto](#criação-de-pasta-para-o-projeto)
2. [Criação do arquivo `index.html`](#criação-do-arquivo-indexhtml)

O projeto pode ser visualizado [clicando aqui](./1_html-and-css-template/)

## Criação de pasta para o projeto

Para inicializar o projeto crie uma pasta raiz No linux, utilizando o terminal execult o comando `mkdir nome-do-projeto`.

## Criação do arquivo `index.html`

Na pasta raiz do projeto, crie uma pasta com o nome `index.html`. Esse arquivo servirá de arquivo raiz para execução e inicialização do projeto.

## Criação das pastas `assets/css`, `assets/img` e `assets/js`.

No diretório raiz do projeto crie as pastas `assets/css`, `assets/img` e `assets/js`. Essas pastas irão organizar os arquivos correspondentes ao seu nome atribuido.

## Criação do arquivo `main.js` na pasta `assets/js` e do arquivo `style.css` na pasta `assets/css`.

Para utilização do javascript no projeto, crie o arquivo `main.js`, este será o arquivo de entrada para os códigos.

Para utilização da estrutura visual proporcionada pelo css, crie o arquivo `style.css` na pasta `assets/css`.

## Escrita inicial da estrutura html do arquivo `index.html`

Escrita inicial html no arquivo da estrutura básica, com link para os arquivos de css e javascript.

### Código

> Arquivo: `projeto/index.html` 

~~~html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modelo HTML e CSS</title>
    <link rel="stylesheet" href="./assets/css/style.css">
</head>

<body>

    <section class="container">
        <h1>Lorem ipsum dolor sit amet.</h1>

        <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Corporis quae ab excepturi velit non eius
            distinctio autem fugiat obcaecati aspernatur.
        </p>

        <form action="">
            <label for="input-teste-1">Label teste #1</label>
            <input type="text" id="input-teste-1">

            <label for="input-teste-2">Label teste #2</label>
            <input type="password" id="input-teste-2">

            <label for="input-teste-3">Label teste #3</label>
            <input type="number" id="input-teste-3">

            <label for="input-teste-4">Label teste #4</label>
            <input type="email" id="input-teste-4">

            <button>Enviar</button>
        </form>

    </section>

    <script src="./assets/js/main.js"></script>
</body>

</html>
~~~

## Escrita inicial da estrutura html do arquivo `style.css` na pasta `assets/css`

Desenvolver o arquivo `.css` para desenvolver o layout da página como desejar.

~~~css
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap');

:root {
    --primary-color: rgb(114, 18, 98);
    --second-color: rgb(77, 12, 66);
    --white: #fff;
}

* {
    box-sizing: border-box;
    outline: 0;
}

body {
    margin: 0;
    padding: 0;
    background: var(--primary-color);
    font-family: 'Open sans', sans-serif;
    font-size: 1.3em;
    line-height: 1.5em;
}

.container {
    max-width: 640px;
    margin: 50px auto;
    background: var(--white);
    padding: 20px;
    border-radius: 10px;
}

form input,
form label,
form button {
    display: block;
    width: 100%;
    margin-bottom: 10px;
}

from input {
    font-size: 24px;
    height: 50px;
    padding: 0 20px;
}

form input:focus {
    outline: 1px solid var(--primary-color);
}

form button {
    border: none;
    background: var(--primary-color);
    color: var(--white);
    font-size: 18px;
    font-weight: 700;
    height: 50px;
    cursor: pointer;
    margin-top: 30px;
}

form button:hover{
    background: var(--second-color);
}
~~~

## Estrutura de Arquivos

~~~txt
projeto
│   index.html
└── assets
    ├── css
    │   └──style.css
    ├── img
    └── js
        └── main.js
~~~
