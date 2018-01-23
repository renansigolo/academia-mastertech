# Back-end: Implementação

### Sintaxe de um Protocolo HTTP

Existem duas coisas bem importantes em uma mensagem HTTP:

* **Header:**

  * Contém as instruções para a transferência das informações que estão contidas no _body_ e até métodos HTTP.

* **Body:**

  * Pode estar vazio ou conter as informações que você deseja transmitir através da rede.

**Exemplo:**

```
Header: Host: localhost:3000
        Connection: keep-alive
        Content-type: application/json
Body:   {
           "nome": "João",
           "idade": 16
        }
```

#### ES6 \(ECMAScript 6\)

O Node utiliza uma versão nova de sintaxe para JavaScript, que contém constantes, _arrow functions_, e várias outras coisas. E para podermos utilizar o Node, precisamos nos adaptar a essas novas variáveis!

* **Constantes:** As constantes têm a mesma função que as variáveis, mas com um único detalhe: quando alocamos um valor à uma constante, não conseguimos mudar mais o valor dela \(por isso que se chamam constantes, né?\). Veja a sintaxe:

```
const minhaConstante = 10;

// Se eu tentar atribuir um outro valor à 'minhaConstante':
minhaConstante = 2.5;

// Não funcionará. O valor será sempre 10.
console.log(minhaConstante); ===> O terminal mostrará 10.
```

* **Arrow functions: **As arrow functions nada mais são do que funções normais, escritas de outra forma. Não há nenhum segredo nelas: só às chamamos de _arrow functions _\(funções flecha\) por causa de sua sintaxe:

```
let minhaFuncao = () => {
    ...
}
```

Segue um exemplo que fizemos em sala de aula:

* Calculando a média utilizando \_arrow functions \_e pegando argumentos através do terminal:

```
let argumentos = process.argv; 
let notas = [];

//Salvando os argumentos pegos pelo terminal no vetor notas: 
for(i = 2; i < argumentos.length; i++){ 
    notas.push(Number(argumentos[i])); 
}

//Função: 
const calcularMedia = (notas) => { 
    let total = 0; 
    for(nota of notas){ 
        total += nota; 
    }

    return total/notas.length;
}

if(calcularMedia(notas) >= 6){ 
    console.log(O aluno foi aprovado com a nota ${calcularMedia(notas)}); 
} else { 
    console.log(O aluno foi reprovado com a nota ${calcularMedia(notas)}); 
}
```

## Beleza, eu aprendi tudo isso. Mas, pra quê?

Nessa semana do _back-end_, vamos aprender a fazer requisições e receber respostas de um servidor usando o Node.js! E para isso precisamos entender primeiro o que são todas essas siglas e termos da Internet. Se olharmos a documentação do Node, as variáveis, constantes, \_arrow functions \_que ele usa possuem nomes específicos que remetem à esses termos. Quer um exemplo? Veja esse código abaixo e tente entender o que ele faz:

    const http = require('http');
    const hostname = '127.0.0.1';
    const port = 3000;

    const server = http.createServer((req, res) => {
        res.statusCode = 200;
        res.setHeader('Content-Type', 'text/plain');
        res.end('Hello World\n');
    });

    server.listen(port, hostname, () => {
        console.log(`Server running at http://${hostname}:${port}`);
    });

### Query Strings

Tudo o que vem depois da "?" é o que chamamos de query string, que são informações que serão interpretadas pela aplicação que é executada no servidor.

![](/assets/tag.jpg)

#### O que é URI?

Um URI \(do inglês Uniform Resource Identifier\) são vários caracteres usados para identificar ou denominar uma aplicação na internet para interagir com representações desta aplicação por intermédio da internet. Um bom exemplo é a URL.

#### 

### Express

O express é um framework de Node.js que é muito utilizado para desenvolver aplicações web que ajuda o node em requisições dos métodos get, post, put já comentados acima. Por exemplo se uma requisição GET fosse feita via Node puro demoraria e o Express vem para ajudar neste processo, pois possui middlewares prontos para serem usados nas requisições.

###### O que é Middleware? é uma função intermediária com acesso ao objeto de requisição \(req\), de resposta \(res\), e ao próximo middleware no ciclo de requisição-resposta de uma aplicação Express. De forma simples:  uma coisa para usar entre/no meio de duas coisas que seriam a requisição e resposta.

Para começar:

```
npm init          //inicia um pacote npm e cria o arquivo package.json
npm install express --save   //instala o express e o save, salva na sua aplicação atual
```

Após instalar é preciso injetar o express em sua aplicação:

```
var express = require('express'),
    app = express();
```

##### 

##### Exemplos do que já foi abordado:

```
const http = require('http');

// Cria servidor
const servidor = http.createServer((req, res) => {
  res.end('Chegou aqui');

});

// Abre porta
servidor.listen(8080);

//rodar npm start
```

API's

API é uma forma de integrar um sistema no outro. Por exemplo o Waze está conectado ao Spotify, então assim autoriza a integração, você o contato com Spotify para navegar, e assim que fizer a "chamada" para ouvir a playlist, ela vai buscar esta lista e começar o streaming, é este processo que chamamos de integração.

