# HTML e CSS

É hora de por a mão na massa e começar a mexer em códigos!

## HTML

HTML é o corpo do seu site, toda a estrutura da página é feito por html. Ele faz o posicionamento de cada item seja título, parágrafo, imagem ou um link. Ele é formado por tags como por exemplo &lt;body&gt; e toda tag deve ser fechada no seu código.

##### ![](/assets/code1.png)

## Tags mais utilizadas no HTML

* `<p>Paragrafo</p>`

* `<h1>Título</h1>`

* `<ul>Lista</ul>`

* `<li>Item da lista</li>`

* `<img src="endereco-da-imagem">`

* `<section> ... <section>`

* `<footer> ... </footer>`

### Form

* Tag de formulário

`<form> </form>`

* Tag do campo de inserção

`<input> <input placeholder="Digite seu nome...">`

* Botão

`<button type="button">Enviar</button>`

### Formulário Completo

```
  <section>
    <form action="/" method="post">
      <input type="text" name="name" placeholder="Digite aqui seu Nome">
      <input type="email" name="email" placeholder="Digite aqui seu Email">
      <input type="password" name="pass" placeholder="Digite aqui sua Senha">
      <button type="button" name="button">Clique aqui para Logar</button>
    </form>
  </section>
```

![](/assets/Screen Shot 2017-11-16 at 3.37.31 pm.png)

### Head

* Exemplo de cabeçalho

```
<head>
    <meta charset="utf-8">
    <title>Nome da Aba do Navegador</title>
    <link rel="stylesheet" href="styles.css">
</head>
```

## CSS

O CSS tem como principal função estilizar seu site, ou seja, deixar ele bonito e personalizado da maneira que você imagina seu site. Ele ajuda também na usabilidade do seu site, e em uma melhor experiência de navegação. A forma de escrever seu CSS é diferente do html, e inserido em um arquivo diferente, geralmente nominado como styles.css.

![](/assets/codecss.png)

## Itens mais utilizados no CSS

* `.classes{  }`

* `#ids{  }`

* `.minha-classe p{  }`

* `display: flex;`

* `position: relative;`

* `position: absolute;`

* `@media(max-width: 600px){}`

## Exemplos de propriedades do CSS

* `color: black`

* `background-color: blue`

* `margin: 0 20px 30px 3px`

* `text-align: center`

## Dicas para o CSS

* Utilizem várias classes em uma mesma tag

```
//HTML
<section class="text-center container">
<h1>Meu Título</h1>
</section>

//CSS
.text-center {
  text-align: center;
}
.container{
  margin: 0 15%;
}
```

* Brinquem com border radius

```
//HTML
<section class="text-center container">
<img src="#" class="bordinha">
<h1>Meu Título</h1>
</section>

//CSS
.text-center {
  text-align: center;
}
.container {
  margin: 0 15%;
}
.bordinha {
  border-radius: 50%;
  border: 1px solid black;
}
```

* Usem o media queries

O que é um media querie?

Uma expressão colocada no seu arquivo CSS que limita/adapta a apresentação do seu conteúdo de acordo com um formato especifica de dispositivos \(tamanho da tela\), geralmente usado para largura, altura e cor.

```
@media(max-width: 1024px) and (min-width: 700px){
  container{
    display: flex;
    }
    h1 {
      color: red;
    }
  }

  @media (max-width: 699px){
    container{
      display: flex;
      flex-wrap: wrap;
      }
      h1 {
        color: blue;
      }
  }
```

## Flexbox

### propriedades Flexbox:

* flex-direction
* flex-wrap
* flex-flow
* justify-content
* align-items
* align-content
* order
* align-self
* flex-grow
* flex-shrink
* flex-basis
* flex

## Hora de colocar em prática seus conhecimentos

Exercício 1

Monte a sua página. Pode ser um currículo, por exemplo uma página com seus hobbies ou coisas preferidas utilizando HTML e CSS.

Exercício 2

Crie uma página que seria um ecommerce. A ideia é ter uma vitrine com produtos e que clicando em algum produto iria para outra página com mais informações sobre este produto. E qual o produto? Você escolhe! Pode ser flores, games, bijouterias...a ideia é estruturar um site com imagens, valores, textos \(pode ser só de marcação\).

