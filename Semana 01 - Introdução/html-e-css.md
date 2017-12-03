# HTML e CSS

É hora de por a mão na massa!

## HTML

HTML é o corpo do seu site, toda a estrutura da página é feito por html. Ele faz o posicionamento de cada item seja título, parágrafo, imagem ou um link. Ele é formado por tags como por exemplo &lt;body&gt; e toda tag deve ser 

## Tags utilizadas no HTML

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

* `.classes{  }`

* `#ids{  }`

* `.minha-classe p{  }`

* `display: flex;`

* `position: relative;`

* `position: absolute;`

* `@media(max-width: 600px){}`

## Propriedades do CSS

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

* Abusem do border radius

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

## 



