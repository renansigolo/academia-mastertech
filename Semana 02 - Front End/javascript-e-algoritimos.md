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

* significa concatenar um elemento ou variável A com o B

++   significa quando vc incrementa/adiciona um valor a variável \(ex: usado no for\)

--    significa quando vc decrementa/diminui um valor a variável

&&   é o mesmo valor de "E".

\|\|    é o mesmo valor de "Ou".

!     é o mesmo valor de "Não".

### Mais exemplos:

* `if(umaCondicao >= queOutra){  };`

* `else(){  };`

* `let titulo = document.querySelector('h1');`

* `let minhaVariavel = 'um valor para esta variável';`

* `funcao nomeDaFuncao(){  }`

* `for (let numero of numeros){ }`

* `console.log(O número ${nomeDaVariavel} é impar);`

* `acumulador = acumulador + numero; == acumulador += numero`

* `<button onclick="minhaFuncao()"> Clique Aqui </button>`

#### For e while

Frequentemente é preciso ter nas aplicações repetir a execução de um bloco de códigos até que determinada condição seja verdadeira, ou senão até uma quantidade de vezes seja o suficiente.

O **while** faz este laço, ou loop de executar o código até que a condição seja verdadeira, porém sem saber o número correto de iterações. Por exemplo, verificar em site de sorteio, se o número 20 foi selecionado. Não está determinado o número de participantes ou de tentativas, então o while vai "rodar" até encontrar este número.

Já o for, também executa o loop porém já está determinado o número de iterações. Por exemplo, usando a mesma ideia do sorteio, é necessário escolher 5 participantes para uma próxima rodada, então já sabemos que o laço irá parar até ter 5 selecionados. Veja o que acontece quando insere este código no console do seu browser:

```
var contador;
for(contador = 0; contador < 10; contador++)
{
  alert(contador);
}
```

### For...of e for...in

Enquanto o`for...in`interage com o nome das propriedades, o`for...of`interage com o valor das propriedades.

```
let vetor = [3, 5, 7];

for (let i in vetor) {
   console.log(i); // logs "0", "1", "2" (aparece a posição de cada vetor ou seja o nome, que neste caso seria números)
}

for (let i of vetor) {
   console.log(i); // logs "3", "5", "7" (neste caso aparece o valor, ou seja a posição 0 tem valor de 3)
}
```

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

## Usando o 'this'

O uso do this é uma forma de referenciar ou criar um atalho para um objeto por exemplo. Uma boa analogia é o uso de pronomes para referenciar o sujeito de uma frase, "João está estudando para evitar que ele fique de recuperação", o ele faria a mesma função do this.

```
let pessoa = {
    Nome : "Bruno",
    Sobrenome: "Pimentel",
    NomeCompleto  : function() {
        //Um exemplo do uso do "this" "ele" referenciando ao objeto pessoa
        console.log( this.Nome + ' ' + this.Sobrenome );

        // Também poderia ter escrito assim:
        console.log( pessoa.Nome + ' ' + pessoa.Sobrenome );
    }
}
```

#### Interpolação

É uma forma mais sucinta para encapsular expressões dentro das strings.

    VERSÃO ANTIGA ES5
    var a = 5;
    var b = 10;
    console.log("Quinze é " + (a + b) + " e não " + (2 * a + b) + ".");
    // "Quinze é 15 e não 20."

    Agora, utilizar as substituções sintaticas torna o código mais legível:
    VERSÃO ANTIGA ES5
    var a = 5;
    var b = 10;
    console.log(`Quinze é ${a + b} e não ${2 * a + b}.`);
    // "Quinze é 15 e não 20."

#### Concatenação

Diferente da matemática, o + não faz a soma em strings, e sim as concatena, como mostra o exemplo abaixo:

```
var palavra1 = "Bom dia";  
var palavra2 = " todo mundo";  
var total = palavra1 + palavra2;     // "Bom dia todo mundo"
```

## Math

Ele é considerado um objeto embutido com propriedades e métodos para constantes e funções matemáticas. Por exemplo para realizar uma exponenciação, é utilizado o método pow `math.pow (x,y)` onde x e y poderia ser 3² \(três elevado a segunda potência\). Ele é um facilitador para realizar operações.

Exemplos:

Math.round\(x\) - Retorna o valor arrendodado de X para o valor inteiro mais próximo.

Math.random\( \) - Retorna um número pseudo-aleatório entre 0 e 1.

### Console

O console é  um objeto com diversos métodos que trabalham em conjunto semelhante ao funcionamento do Math. Ele fornece acesso à consola de depuração do navegador. Um desses métodos mais usado é o log\(\) onde você envia uma informação para depurar o código, verificar onde deu o erro ou em qual parte da função parou de rodar.

Você pode também pode inserir mensagens, como por exemplo com if e else onde você aparece as duas condições que pode acontecer na função.

Exemplo:

```
let apostila = "Academia Mastertech"
console.log (apostila)     // aparece Academia Mastertech.
```

### SetInterval e TimeOut

São duas funções do Javascript que chamamos de temporizadores, e com elas é possível definir um intervalo de tempo em que um evento irá acontecer em milisegundos \(1 segundo = 1000 milisegundos\).

A sintaxe das duas funções é praticamente idêntica, só muda a forma em que elas agem no seu código.

A setTimeout\(\) chama a função uma única vez. Enquanto a setInterval\(\) chama a função “infinitamente” sempre no mesmo intervalo de tempo que é colocado e para pausar a função usa-se clearInterval\(\).

Exemplo para ficar mais claro: Na função abaixo a setInterval\(\) vai executar o que for definido dentro de uma função passada como parâmetro em 50 em 50 milisegundos e este processo vai  durar 3000 milisegundos \(3 segundos\), que é o tempo definido na setTimeout\(\) e ela ai ela para por conta da clearInterval\(\).

```
var intervalo = window.setInterval(function() {
    // inserir uma função aqui
}, 50);

window.setTimeout(function() {
    clearInterval(intervalo);
}, 3000);
```

## Eventos Javascript

Para entender os eventos em JavaScript é legal pensar que estão em camadas. Por exemplo, quando se usa um evento de clique para fazer aparecer uma caixa de diálogo \(`alert()`\), existem uma sequência de ações para acontecer isso.

* Um botão é clicado;
* O botão dispara um evento;
* Algum código está escutando o evento disparado;
* A caixa de diálogo é mostrada "Hello World".

Quando se clica no botão, o navegador emite o que é conhecido como **evento**. Toda a aplicação sabem que o botão foi clicado.. Para ter uma reação a este clique, é preciso que tenha um código que escute este evento para acionar o "disparo" da caixa de diálogo.

Este processo pode ocorrer diversas vezes, ao abrir uma página, clicar em um botão, passar o mouse e dependendo do foco da sua aplicação é preciso escutar o evento certo para atingir a resposta esperada.

Para fazer isso é feito a função addEventListener\(\) onde ela atua como um vigilante 24h que fica de olho em todos os eventos acontecendo em sua aplicação para que possa dar prosseguimento a próxima ação quando o evento for disparado.

Você pode usar a função addEventListener\(\) para escutar os eventos que neste caso é um botão com o id clickButton, que terá o evento click e a função Teste que vai acontecer assim que o clique do botão acontecer e gerar alert com o aviso.

```
<html>
    <head>
        <title>Eventos de Javascript</title>
    </head>

    <body>
        <div id="main">
            <button id="clickButton" class="buttonStyle">clicar aqui</button>
        </div>

        <script>
        let clickButton = document.querySelector("#clickButton");

        clickButton.addEventListener('click', Teste, false);

        function Teste() {
            window.alert("Deu certo!");
        }
        </script>
    </body>
</html>
```

### Alguns eventos mais comuns....

onclick é disparado quando é pressionado e liberado o botão primário do mouse, trackpad, etc.

mousemove é disparado sempre que o cursor do mouse se move.

mouseover é disparado quando o cursor do mouse é movido para sobre algum elemento.

scroll é disparado quando há “rolagem” \(scroll\) num elemento.

## E o que é DOM?

Quando o navegador recebe a requisição e baixa o documento HTML é  preciso transformá-lo em uma página Web que é uma uma longa linha de string de caracteres. E com isso o próprio navegador de inicio decide quais partes são parágrafos, quais são títulos,  e assim por diante e  armazena essa interpretação do código HTML como um estrutura de objetos, chamada **Document Object Model **ou **DOM. **Ele** **cria um objeto diferente para cada elemento, mas vincula cada objeto de elemento ao seu elemento pai. Isso cria uma relação pai-filho como uma estrutura em árvore..![](/assets/tree.png)

#### Maneiras de acessar pelo DOM

| Propriedade | Descrição |
| :--- | :--- |
| documentElement | Captura o elemento raiz &lt;html&gt; de um documento HTML. |
| getElementById | Busca um elemento da página Web com o uso do atributo id do elemento. |
| getElementByClass | Busca um elemento da página Web com o uso da classe do elemento. |
| innerHTML | Retorna ou define o conteúdo de um elemento. |
| appendChild | Insere um novo elemento filho. |
| removeChild | Remove um elemento filho. |

##### _Exercícios resolvidos em sala_

Imprima no console uma escada com a mesma quantidade de degraus que o número contido na variável.

Ex: numero = 4;

\#

\#\#

\#\#\#

\#\#\#\#

```
// ESCADA - forma 1
let numero = 10;   
let degrau = '#';

for(let i = 1; i <= numero; i++){
    degrau += '#';
    console.log(degrau);
}

//ESCADA - forma 2
let escadinha = '#';

let numero_de_degraus = prompt('Digite quantos degraus você deseja: ');

for(let contador = 0; contador < numero_de_degraus; contador++) {
  console.log(escadinha);
  escadinha = escadinha + '#';
}
```

Crie um programa que busque uma letra dentro de uma frase e imprima a quantidade de ocorrências dela, da seguinte forma:

Foram encontradas 4 ocorrências da letra "a" na frase "Colocar dois pratos de trigo para dois tigres".

Não foram encontradas ocorrências da letra "a" na frase "Colocar dois pratos de trigo para dois tigres".

Dica: Em javascript, os caracteres de uma string podem ser acessados usando a notação de vetor.

Por exemplo: considerando que variável palavra contém a string "Facebook", o valor de palavra\[2\] é "c".

    // BUSCA-LETRA
    let frase = "Três pratos de trigo para três tigres tristes";
    let letra_procurada = 'r'
    let contador = 0;


    for(let letra of frase){
        if (letra == letra_procurada){
            contador++;
        }
    }

    console.log(`A frase "${frase}" possui ${contador} letras ${letra_procurada}`);

1- Criar um programa que soma o valor da lista de compra, considerando o  
 valor de cada item e sua quantidade.  
 No final, o programa deve imprimir uma mensagem no console: O valor total da lista de compras é R$ 100.

2- Somar também a quantidade de itens da lista e alterar a mensagem a ser impressa: O valor total da lista de compras é R$ 100 e a quantidade de itens é 23

    let itens = [
      {
        nome: "Banana",
        valor: 2.1,
        quantidade: 1
      },
      {
        nome: "Sabonete",
        valor: 1.3,
        quantidade: 3
      },
      {
        nome: "Doritos",
        valor: 4.7,
        quantidade: 2
      },
      {
        nome: "Pão",
        valor: 0.38,
        quantidade: 10
      },
      {
        nome: "Leite",
        valor: 2.34,
        quantidade: 3
      },
      {
        nome: "Ovos",
        valor: 0.42,
        quantidade: 12
      }
    ];

      let valorTotal = 0;
      let quantidadeProdutos = 0;

      for(let item of itens){
        valorTotal =  Math.ceil(valorTotal)+(item.valor * item.quantidade);
        quantidadeProdutos = quantidadeProdutos + item.quantidade;
      }

      console.log(`O valor total da lista de compras é de R$ ${valorTotal} 
      e a quantidade de produtos é ${quantidadeProdutos}`);

1- Crie um programa que sorteie um dos valores presentes no vetor 'valores'e imprima o resultado no console:  
 _O valor sorteado foi banana.    
_

2- Repita esse sorteio 3 vezes e verifique se os valores sorteados são iguais.  
 Caso sejam, o jogador venceu o jogo. Exemplos de mensagens no console:  
 _Os valores sorteados foram banana, banana e pera. Você perdeu!    
_ e _Os valores sorteados foram banana, banana e banana. Você venceu!_

    let valores = ['maçã', 'banana', 'pera', '7'];
    let escolha = [];



    for(let i = 0; i < 3; i++){
        let x = Math.floor((Math.random() * 4) + 1); //Número aleatório entre 1 e 4
        escolha[i] = valores[x-1];
    }

    if(escolha[0] == escolha[1] && escolha[1] == escolha[2]){
        console.log(`Os valores sorteados foram ${escolha[0]}, ${escolha[1]} e ${escolha[2]}. 
        Parabéns, você foi sorteado!`);
    }
    else {
        console.log(`Os valores sorteados foram ${escolha[0]}, ${escolha[1]} e ${escolha[2]}. 
        Você foi não sorteado!`);

    }

Criar um programa que verifica se um dado vetor está ordenado ou não,  
 e imprima as seguintes mensagens no console.

O vetor está ordenado

O vetor não está ordenado

Obs: O vetor só irá conter números inteiros, positivos e maiores que zero.

    let lista = [10, 20, 50, 100, 1];
    let ok = true;


    for(let item of lista){
        if(lista[item] < lista[item+1]){
            ok = false;
        }
    }

    if(ok == false){
        console.log(`A lista não é ordenada.`);
    }
    else {
        console.log(`A lista é ordenada.`);
    }



