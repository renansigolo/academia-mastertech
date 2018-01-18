# Introdução a programação

## O que é uma linguagem de programação?

Imagine uma linguagem de programação como se fosse um outro idioma.

Assim como nós aprendemos Inglês, Espanhol, Italiano entre outras, as linguagens de programação seguem as mesmas regras e princípios. Quer um exemplo?

Assim como a língua portuguesa é composta da seguinte estrutura, seguindo as regras de sintaxe e semântica, as linguagens de programação funcionam da mesma forma.

![](/assets/sixtaxe.png)

Porém o tempo para se aprender uma linguagem de programação é muito menor do que um outro idioma. Por exemplo_ Python_ que é uma das linguagens mais utilizadas para programar o backEnd contém apenas 33 palavras reservadas. Isso significa que você precisa aprender apenas 33 palavras!

## Conceitos básicos de programação... começando JavaScript

### Variáveis

Variáveis são como caixinhas que armazenam alguma informação dentro delas, em _JavaScript_ nós as declaramos no código da seguinte forma:

```
let nomeDaMinhaVariavel = 'Olá Mastertech';
let numeroNaMinhaVariavel = 7;
let verdadeiroOuFalso = true;
let meuVetor = [34, 23, 53];
let meuObjeto = {
        "nome": "Renan",
        "idade": 26
};
```

Uma variável pode guardar um ou mais elementos dentro dela \(variáveis do tipo Objeto fazem isso\).

### Condições

Podemos controlar nosso código com as estruturas de controle como `if` e `else`

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

Aqui, a variável "palavra" possui valor 'Mastertech'. Quando testamos a condição` if (palavra == 'Banana')`, ela é falsa, e portanto o bloco de código do `if`  não será executado. Ao invés, o bloco de `else` será executado. Esse exemplo deve ser entendido da seguinte forma: _"**Se** palavra for igual a banana, então escreva no console que a palavra é banana. **Senão**, escreva que a palavra não é banana"_.

### Operadores Lógicos

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

### Funções

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

### Loop

Um loop \(laço\) é um conceito de repetição de código onde você continua executando os comandos programados até que uma condição seja atingida.

EXEMPLO 1\)

```
let vetor = [10, 20, 30, 40];

for (let numero of vetor){
      console.log(numero);
} 
```

Nesse exemplo, o console imprimirá todos os valores do vetor.

EXEMPLO 2\)

```
for (let i = 0; i < 10; i++){
    console.log(i);
}
```

Nesse exemplo, o console imprimirá o valor da variável i, desde 0 até 9.

