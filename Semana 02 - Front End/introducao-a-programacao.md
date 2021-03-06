# Introdução a programação - começando JavaScript

## Variáveis e constantes

Em termos simples, são nomes que inventamos para representar um valor, para que assim seja possível usá-lo diversas vezes naquela lista de tarefas, sem precisar reescrevê-lo todas as vezes que ele for necessário. Com o uso de variáveis, utilizamos apenas o nome de referência.

```
let minhaVariável = 'Essa é minha variável e ela guarda essa frase';
```

### Tipos de dados

Quando desenvolvemos programas, geralmente usamos as variáveis para guardas informações sobre o nosso usuário:

* Nome
* Idade
* Salário
* E por aí vai…

Para o computador, tais informações são dados. E dados podem assumir diversos formatos. Pense da seguinte forma, nome é diferente de idade que, por sua vez, é diferente de salário. Isso em lógica de programação pode ser definido como **tipos de dados primitivos**. Estes tipos existem para otimizar a memória do computador, assim, o computador consegue identificar qual é o tipo de dado que ele irá receber/interpretar.

Tratando-se de tipos de dados primitivos, são constatados cinco formatos:

#### Tipo 1: Texto

Os dados do tipo texto representam uma sequência de um ou mais caracteres. São colocados entre aspas dupla ou simples.

Um exemplo de dado do tipo texto:  `let frase = 'As bananas são amarelas';`

**Obs.: **espaços também contam como caracteres.

#### Tipo 2: Números \(inteiros e decimais\)

Os números são o tipo mais básico de dados num programa. Eles podem ser tanto inteiros quanto decimais. Com eles, podemos fazer cálculos numéricos e uma infinidade de outras coisas.

Um exemplo de dado do tipo inteiro: `let idade = 18;`

Exemplo de número decimal: `let salário = 2350.00;`

#### Tipo 3: Lógico

Este tipo de dado normalmente é representado por alternativas: SIM ou NÃO, VERDADEIRO ou FALSO. Dados do tipo lógico também podem são chamados de booleano \(em homenagem à George Boole, que criou esse tipo de lógica\).

Um exemplo de dado lógico que é frequentemente utilizado em programação é para verificar se situações são verdadeiras ou 9falsas: `let estouComSono = false;`

#### Tipo 4: Vetores

Os vetores são um método prático de guardar vários dados em uma mesma variável. Por exemplo:

```
let numero = 15;
let palavra = banana;
let booleano = true;
```

Podemos facilmente guardar esses números utilizando somente uma variável:

```
let vetor = [15, 'banana', true];
```

E acessamos essas variáveis indicando ao programa qual o índice dentro do vetor em que ela está posicionada:

```
vetor[0] == 15
vetor[1] == 'banana'
vetor[2] == true
```

**Importante:** os vetores **sempre** iniciam os índices em 0.

#### Tipo 5: Objetos

Um objeto é uma coleção de propriedades, em que cada propriedade possui um par chave =&gt; valor. Os objetos de programação podem ser comparados com os objetos na vida real: por exemplo, um carro possui as seguintes propriedades: motor, janelas, uma cor de tintura, um peso, etc...

Em um programa definimos um objeto da seguinte forma:

```
let carro = {
    motor: true,
    janelas: 4,
    cor: preto,
    peso: 1000
}
```

**Obs.:** Você deve ter percebido que colocamos as variáveis com a seguinte sintaxe:

`let <NomeDaVariável> = <Valor da variável>;`

Essa é a sintaxe que usamos no _JavaScript_ para declarar variáveis.

## Condições

Podemos controlar nosso código com as estruturas de controle como `if`, `else` e `else if`

Elas servem para filtrar o resultado caso a condição definida seja verdadeira, veja os exemplos abaixo:

EXEMPLO 1\)

    let numero = 2;

    if (numero == 2) {
     console.log(`Esse número vale 2!`);
    }
    else {
     console.log(`O número não vale 2.`);
     }

Nesse exemplo, a variável "numero" possui valor 2. Quando testamos a condição `if (numero == 2)`, ela é verdadeira, e portanto o código que está dentro das chaves \(`{ }`\) dessa condição será executado. Esse exemplo deve ser entendido da seguinte forma: "_**Se** o numero for igual a 2, escreva no console que ele vale 2. **Senão**, escreva que ele não vale 2_".

EXEMPLO 2\)

    let palavra = 'Mastertech';

    if (palavra == 'Banana') {
        console.log(`A palavra é banana!`);
    }
    else {
        console.log(`A palavra não é banana.`);
    }

Aqui, a variável "palavra" possui valor 'Mastertech'. Quando testamos a condição`if (palavra == 'Banana')`, ela é falsa, e portanto o bloco de código do `if`  não será executado. Ao invés, o bloco de `else` será executado. Esse exemplo deve ser entendido da seguinte forma: _"**Se** palavra for igual a banana, então escreva no console que a palavra é banana. **Senão**, escreva que a palavra não é banana"_.

EXEMPLO 3\)

    let numero = 15;

    if(numero < 5){
        console.log(`O número é menor do que 5`);
    }
    else if(numero == 10){
        console.log(`O número é igual a 10!`);
    }
    else {
        console.log(`O número não é menor que cinco e nem é igual a 10.`);
    }

Leia-se: "**Se** o número for menor do que cinco, execute o primeiro _console.log_. **Senão**, verifique se ele é igual a 10. **Se sim**, execute o segundo _console.log_. **Senão**, execute o terceiro e último _console.log_". Quando precisamos verificar mais de uma condição, e para cada condição executamos códigos diferentes, utilizamos o `else if`. Podemos utilizar quantos `else if` quisermos em nosso código, mas somente um `else`.

## Operadores Lógicos

As expressões `if` e `else` são usadas para testar condições lógicas simples. Quando precisamos testar a validade de operações lógicas mais complexas, podemos fazer isso com os operadores lógicos. São eles:

* `!=` - NÃO lógico, operador de negação;
* `&&` - E lógico, operador de conjunção;
* `||` - OU lógico, operador de disjunção;
* `==` - Operador de comparação.

Elas também servem para filtrar o resultado caso a condição definida seja verdadeira, veja os exemplos abaixo:

EXEMPLO 1\)

    let numero = 2;
    let palavra = 'mastertech';

    if (numero != 2){
        console.log(`O numero não é 2!`);
    }

Leia-se: "_**Se** o numero **não** for 2, então imprima no console que ele não vale 2_". A variável "numero" vale 2, e portanto o bloco de código não será executado.

EXEMPLO 2\)

    let numero = 2;
    let palavra = 'mastertech';

    if (numero == 2 && palavra == 'mastertech'){
        console.log(`O numero vale 2 e a palavra é mastertech!`);
    }

Leia-se: "_**Se** o numero for igual a 2 **e** se a palavra for igual a mastertech, então imprima no console_".

EXEMPLO 3\)

    let numero = 2;
    let palavra = 'mastertech';

    if(numero == 2 || palavra == 'banana'){
        console.log(`Uma das afirmações está correta!`);
    }

Leia-se: "_**Se** o numero for igual a 2 **ou** a palavra for igual a banana, então imprima no console_". No caso, a variável "numero" equivale a 2, mas a variável "palavra" não equivale a banana. Com o operador lógico OU, somente uma das afirmações precisa ser verdadeira para que o bloco de código seja executado.

## Operadores Matemáticos

Existem operadores matemáticos básicos que podemos usar em nossos programas para fazer cálculos matemáticos simples: somar, subtrair, dividir, multiplicar e afins. São eles:

* `+` - somar;
* `-` - subtrair;
* `/` - dividir;
* `*` - multiplicar;
* `>` e `>=` - maior e maior ou igual;
* `<` e `<=` - menor e menor ou igual;
* `++` - somar 1 ao valor da variável;
* `--` - subtrair 1 ao valor da variável;
* `+=` - adicionar à variável um valor;
* `-=` - subtrair da variável um valor;
* `*=` - multiplicar o valor da variável por um valor dado.

Seguem alguns exemplos :

EXEMPLO 1\)

```
let i = 0;
i++; //Soma 1 ao valor de i: i + 1 = 0 + 1 = 1

let a = 5;
a += 10; //Soma 10 ao valor de a: a + 10 = 5 + 10 = 15

let b = 6;
let c = 10;
c > b = true //10 é menor que 6, então é uma afirmação verdadeira
```

## Laços de repetição

Um _loop_ \(laço\) é um conceito de repetição de código onde você continua executando os comandos programados até que uma condição seja atingida. Os laços sempre possuem uma variável "contadora", que usamos como referência para saber em qual laço estamos \(por exemplo, podemos começar do 0 e fazer um laço de repetição que repita nosso código 10 vezes\). Existem dois tipos de laços: o primeiro usa como referência um vetor, passando por casa um de seus itens e realizando cálculos com eles.

No outro, usamos uma variável criada dentro do laço, colocamos uma "condição de parada" \(alguma afirmação que seja verdadeira para fazer o laço continuar rodando, e que fique falsa quando queremos que o laço pare\), e incrementamos sempre o valor dessa variável em 1. Veja exemplos:

EXEMPLO 1\)

```
let vetor = [10, 20, 30, 40];

for (let numero of vetor){
      console.log(numero);
}
```

Nesse exemplo, o console imprimirá todos os valores do vetor, e o laço parará de rodar quando chegar ao final do vetor.

EXEMPLO 2\)

```
for (let i = 0; i < 10; i++){ //(for(variável contadora de iterações; condição de parada; incremento){ }
    console.log(i);
}
```

Nesse exemplo, o console imprimirá o valor da variável i, desde 0 até 9.

#### O laço while

O **while** faz este laço \(_loop\)_ de executar o código até que a condição seja verdadeira, porém sem saber o número correto de iterações. Por exemplo, verificar em site de sorteio, se o número 20 foi selecionado. Não está determinado o número de participantes ou de tentativas, então o _while_ vai executar até encontrar este número.

```
var contador = 100;

while (contador > 0){
    console.log(contador);
    contador--;
}
```

#### For...of e for...in

Enquanto o `for...in` interage com o nome das propriedades, o `for...of` interage com o valor das propriedades:

```
let vetor = [3, 5, 7];

for (let i in vetor) {
   console.log(i); // logs "0", "1", "2" (aparece a posição de cada vetor ou seja o nome, que neste caso seria números)
}

for (let i of vetor) {
   console.log(i); // logs "3", "5", "7" (neste caso aparece o valor, ou seja a posição 0 tem valor de 3)
}
```

## Funções

Funções são uma forma de se estruturar sua aplicação para que você reutilize um mesmo código em diferentes lugares, desta forma nós não precisamos ficar reescrevendo o mesmo código cada vez que  precisarmos utilizá-lo. Determinamos a função como o "cabeçalho" do código que vamos reutilizar, e podemos chamá-lo em qualquer parte do código.

Veja o exemplo abaixo:

    // Determinando o cabeçalho da função:
    function minhaFuncao(){
        console.log(`Você chamou a função minhaFuncao!`);
    }

    // Chamando a função no código:
    minhaFuncao();

**Parâmetros:** é possível definir parâmetros para suas funções. Com eles, podemos utilizar o mesmo bloco de função para valores diferentes: a cada vez que chamarmos a função, podemos colocar valores diferentes e cada uma executará com o parâmetro que foi dado. Veja o exemplo:

    // Definindo o cabeçalho da função:
    function fazerMilkshake(sabor){
        console.log(`Por favor, eu quero um milkshake de ${sabor}!`);
    }

    // Chamando a função no código, com parâmetros:
    fazerMilkshake(morango);
    fazerMilkshake(chocolate);
    fazerMilkshake(ovomaltine);

Nessa execução, o console nos mostrará o seguinte:

* "Por favor, eu quero um milkshake de morango!"
* "Por favor, eu quero um milkshake de chocolate!"
* "Por favor, eu quero um milkshake de ovomaltine!"



