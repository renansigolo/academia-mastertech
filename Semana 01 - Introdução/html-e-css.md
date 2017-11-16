# HTML e CSS

É hora de por a mão na massa!

## HTML

* `<form> </form>`

* `<input> <input placeholder="Digite seu nome...">`

* `<button type="button" onclick="alternarModal()">Enviar</button>`

* `<link src="styles.css">`

* `<section> <section>`

* `<footer> </footer>`

* `<button onclick="minhaFuncao()"> Clique Aqui </button>`

## CSS

* `.classes{  }`

* `#ids{  }`

* `.minha-classe p{  }`

* `display: flex;`

* `position: relative;`

* `position: absolute;`

* `@media(max-width: 600px){}`

## Tags utilizadas no HTML

* `<p>Paragrafo</p>`

* `<h1>Título</h1>`

* `<ul>Lista</ul>`

* `<li>Item da lista</li>`

* `<img src="endereco-da-imagem">`

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



