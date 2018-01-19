# Bora aprender o que é o tão falado Javascript

A primeira coisa que você precisa saber, e que vai mudar a sua vida: _JavaScript_ não tem nada a ver com _Java_.

_Java_ é uma outra linguagem de programação usada mais em _back-end_, como _PHP, Ruby, Python_. Já o _JavaScript_ é uma linguagem de programação _client-side_, ou seja usada em _front-end_ para controlar o HTML e o CSS e manipular o comportamento da sua página.

Exemplo: quando você passa o mouse em um menu e de forma mágica aparece um submenu com outros itens, adivinha quem fez isso? O _JavaScript_, que  é executado e faz a função de esconder e mostrar aquele submenu.

Quer um exemplo básico, insira este código no Sublime e abra o arquivo HTML no seu navegador.

![](/assets/Screen Shot 2017-12-13 at 8.28.11 AM.png)

## Relembrando...

* `if(umaCondicao >= queOutra){  };`

* `else(){  };`

* `let minhaVariavel = 'um valor para esta variável';`

* `funcao nomeDaFuncao(){  }`

* `for (let numero of numeros){ }`

* `console.log(O número ${nomeDaVariavel} é impar);`

* `acumulador = acumulador + numero; == acumulador += numero`

## Utilizando JavaScript com HTML e CSS

#### Colocando um arquivo script.js em seu HTML

Para que seu _HTML_ e _CSS_ identifiquem as funções que temos no nosso script, precisamos acrescentar ao final do nosso &lt;body&gt;&lt;/body&gt; a seguinte linha de código:

```
<script src="script.js"></script>
```

#### Mexendo com elementos do HTML no JavaScript

Para de fato conseguirmos realizar qualquer tipo de programação em nosso _HTML_, precisamos selecionar e identificar no script com qual elemento vamos mexer. Para isso, usamos:

```
let meuElemento = document.querySelector(seletor);

ou

let meusElementos = document.querySelectorAll(seletor);
```

#### Inserindo uma função em um botão

![](/assets/button-testejs.png)

Criando um botão via HTML, quando você tenta clicar nele nada acontece. Por isso podemos inserir uma função de clique neste botão. Insira a função abaixo e teste em seu navegador.

```
<!DOCTYPE html>
<html>
<link rel="stylesheet" href="css/styles.css">

<head>
    <meta charset="utf-8">
    <title>Mastertech</title>
</head>

<h1> Academia Mastertech </h1>
<p> Começando a programar </p>

<button onclick="clicar()"> Clique Aqui </button>

<script src="js/script.js"></script>
</body>

</html>

//arquivo js//

function clicar(){
    alert("teste com sucesso");
}
```

## Brincando com o Javascript - Botão

Para inserir um conteúdo em um formulário e alterar em seu site é simples de fazer pelo _JavaScript_. Veja este exemplo:

No arquivo _HTML_, inserimos um novo item &lt;p&gt;, &lt;input&gt; e &lt;button&gt; com id e no botão chamando a função do JS.

![](/assets/fucntion-teste.png)

Já no arquivo script.js inserimos uma nova função, a 'mudarTexto' onde será o start para alterar o texto de seu HTML de acordo com o que for inserido no campo do formulário.

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

        clickButton.addEventListener('click', Teste);

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

### Exercícios para relembrar...

1 - Declare uma variável x com um valor inteiro entre 0 e 10. Se o valor for maior que 5, imprima "Maior que 5",  
se for menor que 5, imprima "Menor que 5" e se for igual a 5, imprima "Igual a 5".

```
var x = 3;

if ( x > 5 )

print("Maior que 5");

else if ( x < 5 )

print("Menor que 5");

else

print("Igual a 5");
```

2 - Crie uma função e declare dentro dela duas variáveis: uma contendo seu nome e na outra seu sobrenome. Quando

```
chamada, essa função deve imprimir "Eu sou &lt;nome&gt; &lt;sobrenome&gt;, e estou na Estação Hack". OBS: Você deve utilizar

as variáveis quando for imprimir.
```

```
function(nome, sobrenome){

print("Eu sou "+nome+" "+sobrenome+", e estou na Estação Hack");

}
```

3 - Crie um botão que quando clicado exibe uma caixa de mensagem com o conteúdo "Olá Estação Hack!"

```
<!doctype html>
<html>
  <body>
    <button type="button" id="botao">Click Me!</button>
  </body>
  <script>
    var botao = document.getElementById("botao");
    botao.onclick = function(){
      alert("Olá Estação Hack!");
    }
  </script>
</html>
```

##### 

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



