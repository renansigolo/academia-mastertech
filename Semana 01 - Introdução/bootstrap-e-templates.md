# Bootstrap e templates

## O que é?

###### _“Projetado para qualquer um em qualquer lugar”_

um **framework **para front-end criado para facilitar e ajudar no trabalho do DEV, oferecendo padrões para HTML, JavaScript e CSS para criações de páginas web de maneira responsiva e gratuita.

##### Mas o que é um Framework mesmo? Imagina um quebra-cabeça. Há várias peçinhas já com uma identidade, cor, desenho, formato e que juntas formam uma imagem. É a mesma coisa, são conjuntos de códigos já criados e testados que juntos criam o seu site.

## Como Instalar o Bootstrap4?

Nós temos algumas opções nas formas de incluir o Bootstrap em nosso projeto.

### Bootstrap4 \(beta 2\) - via CDN

* Insere o Bootstrap 4 através de CDN no seu projeto

`<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css" integrity="sha384-PsH8R72JQ3SOdhVi3uxftmaW6Vc51MKb0q5P2rRUpPvrszuE4W1povHYgTpBfshb" crossorigin="anonymous">`

* Insere o JS do Bootstrap via CDN em seu projeto

```
<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.3/umd/popper.min.js" integrity="sha384-vFJXuSJphROIrBnz7yo7oB41mKfc8JzQZiCq4NCceLEaO4IHwicKwpJf9c9IpFgh" crossorigin="anonymous"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/js/bootstrap.min.js" integrity="sha384-alpBpkh1PFOepccYVYDB4do5UnbKysX5WZXm3XxPqe5iKTfUKjNkCk9SaVuEZflJ" crossorigin="anonymous"></script>
```

### Bootstrap4 \(beta 2\) - via NPM

* Instale o Bootstrap 4 através do NPM \(Package Manager\)

```
npm install bootstrap@4.0.0-beta.2
```

* Instale outras dependências para rodar o JS do bootstrap

```
npm install jquery

npm install popper.js
```

## O que é Bootstrap?

###### _“Projetado para qualquer um em qualquer lugar”_

um **framework **para front-end criado para facilitar e ajudar no trabalho do DEV, oferecendo padrões para HTML, JavaScript e CSS para criações de páginas web de maneira responsiva e gratuita.

##### Mas o que é um Framework mesmo? Imagina um quebra-cabeça. Há várias peçinhas já com uma identidade, cor, desenho, formato e que juntas formam uma imagem. É a mesma coisa, são conjuntos de códigos já criados e testados que juntos criam o seu site.

Link para referenciar no seu html

```
versão 3.3.7
https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css

versão 4 beta (que estamos usando no curso)
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.3/css/bootstrap.min.css" 
rel="stylesheet" integrity="sha384-Zug+QiDoJOrZ5t4lssLdxGhVrurbmBWopoEl+M6BdEfwnCJZtKxi1KgxUyJq13dy" 
crossorigin="anonymous">
```

Incluir a linha abaixo também que é a meta tag de viewport que faz o site ocupar todo o espaço disponível na janela, tanto em celulares, como em tablets ou em PC, e é ela que possibilita o design responsivo e o mobile-first. Pode ser usada tanto no bootstrap como em qualquer outro site.

```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

#### Grids

O grid do Bootstrap funciona assim:

* Colunas `.col`devem estar dentro de linhas `.row`que por sua vez devem estar dentro de um`.container`\(largura fixa\) ou  
  `.container-fluid`\(largura total\).

* Colunas são criadas obedecendo o critério de múltiplos de 12 e este é valor total do seu site. Por exemplo, três colunas de largura equivalentes devem ter a classe`.col-**-4`\(4 + 4 + 4 = 12\). É como uma planilha de excel que tenha apenas 12 colunas que você possa trabalhar.

* Se mais de 12 colunas forem colocadas dentro de uma única linha, uma nova linha abaixo da atual comportará as demais colunas.

* As colunas possuem classes que variam de acordo com o dispositivo e podem trabalhar com outras classes em paralelo a ela. Segue uma figura que exemplifica as classes mas há também a documentação que mostra exatamente como ficaria cad linha de acordo com o que foi definido de comportamento para a coluna.

Além do grid, o bootstrap possui várias classes com atributos de CSS já definidos para facilitar na hora de criar um site responsivo. Tanto é possível criar um site inteiro só com Boostrap como também personalizar alguns itens através do seu arquivo CSS.

O importante neste caso é inserir o link do seu CSS após o link do Boostrap, assim por ordem de leitura do navegador o seu CSS será o último e considerado como o final.

Como exercício, temos um página já criada com elementos e que precisa de melhorias. Baixe o projeto no seu computador e começe a sua página em Boostrap.

Endereço: [https://github.com/Diandralas/semana1](https://github.com/Diandralas/semana1-hack)



