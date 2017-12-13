# Bora aprender o que é o tão falado Javascript.

A primeira coisa que você precisa saber, e que vai mudar a sua vida: JavaScript não tem nada a ver com Java.

Java é uma outra linguagem de programação usada mais em back-end, como PHP, Ruby, Python. Já o JavaScript é uma linguagem de programação client-side, ou seja usada em front-end para controlar o HTML e o CSS e manipular o comportamento da sua página, ou seja, ela é responder por trazer mágica a sua página.

Exemplo: Quando você passa o mouse em um menu e de forma mágica aparece um submenu com outros itens, adivinha quem fez isso? O Javascript, que  é executado e faz a função de esconder e mostrar aquele submenu.

Quer um exemplo básico, insira este código no Sublime e abra o arquivo html no seu navegador.

![](/assets/Screen Shot 2017-12-13 at 8.28.11 AM.png)

## exemplos JS

* Operadores `>, <, =<, >=, ==, !=`

* `if(umaCondicao >= queOutra){  };`

* `else(){  };`

* `let titulo = document.querySelector('h1');`

* `let minhaVariavel = 'um valor';`

* `funcao nomeDaFuncao(){  };`

* `titulo.innerHTML = 'um texto qualquer';`

* `let numeros = [90, 10, 21, 2, 72, 5, 7];`

* `for (let numero of numeros){ }`

* `console.log(O número ${nomeDaVariavel} é impar);`

* `acumulador = acumulador + numero; == acumulador += numero`

* `<button onclick="minhaFuncao()"> Clique Aqui </button>`

## ES5 x ES6

* Duas formas de declarar uma função \(Ambos são a mesma coisa!!! Elas somente estão escritas de formas diferentes\)

ES5

```
function defineNome(){

}
```

ES6

```
const defineNome = () => {

}
```

## O que é DOM?

Ele é uma representação da sua página no navegador como se fosse uma árvore. Ele que define métodos para acessar à sua árvore, assim é possível alterar a estrutura, estilo e conteúdo........???

| Propriedade | Descrição |
| :--- | :--- |
| documentElement | Captura o elemento raiz &lt;html&gt; de um documento HTML. |
| getElementById | Busca um elemento da página Web com o uso do atributo id do elemento. |
| getElementByClass | Busca um elemento da página Web com o uso da classe do elemento. |
| innerHTML | Retorna ou define o conteúdo de um elemento. |
| appendChild | Insere um novo elemento filho. |
| removeChild | Remove um elemento filho.  |



