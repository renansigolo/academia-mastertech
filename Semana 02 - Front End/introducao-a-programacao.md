# Introdução a programação - Renan

## O que uma linguagem de programação?

Linguagem de programação nada mais é do que uma outra língua.

Assim como nós aprendemos Inglês, Espanhol, Italiano entre outras,  as linguagens de programação seguem as mesmas regras e princípios. Quer um exemplo...

Assim como a língua portuguesa é composta da seguinte estrutura seguindo as regras de sintaxe e semântica, as linguagens de programação funcionam da mesma forma.

![](/assets/sixtaxe.png)

Porém o tempo para se aprender uma linguagem de programação é muito menor do que um outro idioma. Por exemplo Python que é uma das linguagens mais utilizadas para programar o backEnd contém apenas 33 palavras reservadas. Isso significa que você precisa aprender apenas 33 palavras!

![](/assets/lang.png)

## Conceitos básicos de programação

### Variáveis

Variáveis são como caixinhas que armazenam alguma informação dentro delas, em javascript podemos demonstrar da seguinte forma:

```
let nomeDaMinhaVariavel = 'Olá Mastertech'
let numeroNaMinhaVariavel = 7
let verdadeiroOuFalso = true
let meuArray = [34, 23, 53]
let meu Objeto = {
        "nome": "Renan",
        "idade": 26
}
```

Uma variável pode guardar um ou mais elementos dentro dela

### Funções

Funções são uma forma de se estruturar sua aplicação para que você reutilize um mesmo código em diferentes lugares, desta forma nós não precisamos ficar reescrevendo o mesmo código cada vez que  precisarmos utilizá-lo

Veja o exemplo abaixo

```
const nomeDaMinhaFuncao = (  ) => {
    
    let meuObjeto = {
        "nome": "Renan",
        "idade": 26
    }
}

```

### Loop

Um loop é um conceito de repetição de código onde você continua executando os comandos programados até que uma condição seja atingida.

```
const multiplosDeDez = (  ) => {
    let a = [10, 20, 30, 40];

    for (let e of a){
      console.log(e);
}

const contarAteDez = (  ) => {
    var a = 1;

    while (a < 10) {
      ++a;
      console.log(a);
    }    
}

```



