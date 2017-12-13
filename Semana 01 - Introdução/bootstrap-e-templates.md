# Bootstrap e templates

## O que é?

###### _“Projetado para qualquer um em qualquer lugar”_

um **framework **para front-end criado para facilitar e ajudar no trabalho do DEV, oferecendo padrões para HTML, JavaScript e CSS para criações de páginas web de maneira responsiva e gratuita.

##### Mas o que é um Framework mesmo? Imagina um quebra-cabeça. Há várias peçinhas já com uma identidade, cor, desenho, formato e que juntas formam uma imagem. É a mesma coisa, são conjuntos de códigos já criados e testados que juntos criam o seu site.

## Como Instalar o Bootstrap4?

Nós temos algumas opções nas formas de incluir o Bootstrap em nosso projeto.

### Bootstrap4 \(beta 2\) - CDN

* Insere o Bootstrap 4 através de CDN no seu projeto

`<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css" integrity="sha384-PsH8R72JQ3SOdhVi3uxftmaW6Vc51MKb0q5P2rRUpPvrszuE4W1povHYgTpBfshb" crossorigin="anonymous">`

* Insere o JS do Bootstrap via CDN em seu projeto

```
<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.3/umd/popper.min.js" integrity="sha384-vFJXuSJphROIrBnz7yo7oB41mKfc8JzQZiCq4NCceLEaO4IHwicKwpJf9c9IpFgh" crossorigin="anonymous"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/js/bootstrap.min.js" integrity="sha384-alpBpkh1PFOepccYVYDB4do5UnbKysX5WZXm3XxPqe5iKTfUKjNkCk9SaVuEZflJ" crossorigin="anonymous"></script>
```

### Bootstrap4 \(beta 2\) - NPM

* Instale o Bootstrap 4 através do NPM \(Package Manager\)

```
npm install bootstrap@4.0.0-beta.2
```

* Instale outras dependências para rodar o JS do bootstrap

```
npm install jquery

npm install popper.js
```

### Bootstrap4 \(beta 2\) - Yarn

* Instale o Bootstrap 4 através do YARN \(Package Manager\)

```
yarn add bootstrap@4.0.0-beta.2
```

* Instale outras dependências para rodar o JS do bootstrap

```
yarn add jquery

yarn add popper.js
```

> Após adicionar as dependências ao seu projeto certifique-se de que você está importando os arquivos de seus locais corretos
>
> // CAMINHOS DAS BIBLIOTECAS EM SUAS RESPECTIVAS ORDENS \(JQUERY, POPPER, BOOTSTRAP\)
>
> 'node\_modules/jquery/dist/jquery.slim.min.js',
>
> 'node\_modules/popper.js/dist/umd/popper.min.js',
>
> 'node\_modules/bootstrap/dist/js/bootstrap.min.js'

### Download Manual

* Baixe os arquivos através do [link](https://getbootstrap.com/docs/4.0/getting-started/download/)

* Descompacte o arquivo `.zip`

* Mova os arquivos para dentro do seu projeto

* Importe em seus respectivos locais



