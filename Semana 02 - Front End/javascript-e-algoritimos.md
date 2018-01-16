# Bora aprender o que é o tão falado Javascript.

A primeira coisa que você precisa saber, e que vai mudar a sua vida: JavaScript não tem nada a ver com Java.

Java é uma outra linguagem de programação usada mais em back-end, como PHP, Ruby, Python. Já o JavaScript é uma linguagem de programação client-side, ou seja usada em front-end para controlar o HTML e o CSS e manipular o comportamento da sua página, ou seja, ela é responder por trazer mágica a sua página.

Exemplo: Quando você passa o mouse em um menu e de forma mágica aparece um submenu com outros itens, adivinha quem fez isso? O Javascript, que  é executado e faz a função de esconder e mostrar aquele submenu.

Quer um exemplo básico, insira este código no Sublime e abra o arquivo html no seu navegador.

![](/assets/Screen Shot 2017-12-13 at 8.28.11 AM.png)

## JavaScript

## Valores

O JavaScript reconhece os seguintes tipos de valores:

* Números** **: como 42 ou 3,14159
* Valores lógicos chamados de Booleanos: true ou false

![](/assets/boolean.png)

* Strings: como "Mastertech!" ou "guarda-roupa"
* null :  um valor nulo;
* undefined: uma propriedade que possui o valor indefinido;

### Tipos de dados abstratos/agrupados

objetos - é como um dado que tem propriedades. Compare-o com um carro, por exemplo. Um carro tem uma cor, um modelo, peso, um ano de fabricação, etc. Da mesma forma, objetos em JavaScript podem ter propriedades, que definem suas características.

vetor \[ \] - é um agrupamento de variavéis, e sempre começa em zero. As variavéis tanto podem ser strings, números, booleanos....O mais comum é verificar vetores com um mesmo tipo, por exemplo, um vetor de nomes, só teria strings.![](/assets/2018-01-15 %282%29.png)

![](/assets/2018-01-15 %282%29.png)

#### Função é diferente de objeto

_Os objetos são como nome da caixinha que vai ser guardado os valores, e funções são como um passo a passo do que a sua aplicação vai executar._

### Variavéis

Variáveis são como nomes simbólicos para os valores em sua aplicação,imagina que você vai trabalhar com várias variavéis, e não pode todas terem o nome de strings ou de números.

Há variáveis globais e locais, sendo que a principal diferença entre elas é onde são declaradas e  sua validade. Como assim?

Uma variável global é declarada em um objeto global, que será válido para todo o documento, e uma variável local geralmente fica armazenada dentro de uma função e quando esta função termina, aquela variável morre. Você não consegue a utilizar em outra função como ocorre com uma global.

Para declarar uma variável \(local e global\) pode-se  colocar :

`var Idade : 20;`

`var Nome: "João";`

Ou sem a palavra var, que ficaria como:

`Nome: "João"`

## exemplos JS

#### Operadores 

=  significa atribuir um valor a uma variável

== significa Igual.

!=  significa Diferente.

=== significa Estritamente igual \(verifica conteúdo e tipo da variável\).

!==  significa Estritamente diferente \(verifica conteúdo e tipo da variável\);

&lt;    Menor que.

&lt;=  Menor ou igual a.

&gt;    Maior que.

&gt;=  Maior ou igual a.

+    significa concatenar um elemento ou variável A com o B

++   significa quando vc incrementa/adiciona um valor a variável \(ex: usado no for\)

--    significa quando vc decrementa/diminui um valor a variável 

&&   é o mesmo valor de "E".

\|\|    é o mesmo valor de "Ou".

!     é o mesmo valor de "Não".



### Mais exemplos:

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

if e else

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

## Exemplos básicos de funções

Inserindo uma função em um botão![](/assets/button-testejs.png)Criando um botão via html, quando você tenta clicar nele nada acontece. Por isso podemos inserir uma função de clique neste botão. Insira a função abaixo e teste em seu navegador.

```
<!DOCTYPE html>
<html>
<link rel="stylesheet" href="css/styles.css">

<head>
    <meta charset="utf-8">
    <title>Mastertech</title>
</head>

<h1> Academia Mastertech</h1>
<p> Começando a programar</p>

<button onclick="Clicar()">Clique Aqui</button>

<script type="text/javascript" src="js/script.js"></script>
</body>

</html>

//arquivo js//

function Clicar(){
alert("teste com sucesso");
}
```

## Brincando com o Javascript - Botão

Para inserir um conteúdo em um formulário e alterar em seu site é simples de fazer pelo Javascript. Veja este exemplo:

No arquivo html, inserimos um novo item &lt;p&gt;, &lt;input&gt; e &lt;button&gt; com id e no botão chamando a função do JS.

![](/assets/fucntion-teste.png)

Já no arquivo script.js inserimos uma nova função, a 'MudarTexto' onde será o start para alterar o texto de seu html de acordo com o que for inserido no campo do formulário.

Criamos uma nova variável para armazenar o valor \(value\) que será "recebido" do campo &lt;input&gt;. E logo em seguida, busca um elemento que está no arquivo html, com um id que é colocado \(' '\) e receberá o valor da variável colocada acima.

Teste e veja o que acontece no seu navegador.

![](/assets/fucntion-teste2.png)

\*\*Tente inserir dentro da função o seguinte trecho:

```
document.getElementById('novotexto').style.color = "orange";
```

## E o que é DOM?

Ele é uma representação da sua página no navegador como se fosse uma árvore. Ele que define métodos para acessar à sua árvore, assim é possível alterar a estrutura, estilo e conteúdo.![](/assets/tree.png)

| Propriedade | Descrição |
| :--- | :--- |
| documentElement | Captura o elemento raiz &lt;html&gt; de um documento HTML. |
| getElementById | Busca um elemento da página Web com o uso do atributo id do elemento. |
| getElementByClass | Busca um elemento da página Web com o uso da classe do elemento. |
| innerHTML | Retorna ou define o conteúdo de um elemento. |
| appendChild | Insere um novo elemento filho. |
| removeChild | Remove um elemento filho. |



