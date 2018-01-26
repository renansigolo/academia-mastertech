# Exemplo Prático: utilizando os conceitos dessa semana

Vamos montar aqui um exemplo prático usando Node.js, Express.js e MongoDB para fazer requisições GET e POST.

* Vamos criar uma pasta em nosso Desktop, chama `minha-api`

![](/assets/exemplo-img-1.PNG)

* Dentro dela, vamos criar nosso arquivo `index.js`. Podemos criá-la direto no Visual Studio Code:

![](/assets/exemplo-img-2.PNG)

* Antes de executar qualquer código, precisamos iniciar o Node.js. Para isso, utilizamos o comando `npm init`. Podemos fazê-lo direto no terminal do VS Code:

![](/assets/exemplo-img-3.PNG)

> Esse comando iniciará o Node.js e o NPM, e criará um arquivo chamado `package.json` com as configurações do nosso projeto. Vamos instalar agora o Express.js.
>
> **Relembrando: **Express.js é um framework para criar aplicações web usando o Node como base. Ela simplifica o processo de criação de um servidor, que já está disponível no Node puro \(para relembrar: O Node permite que usemos JavaScript no back-end de nossas aplicações\).

* Rodamos o código no terminal:

![](/assets/exemplo-img-4.PNG)

* E vamos indicar no nosso index.js que usaremos o Express:

![](/assets/exemplo-img-5.PNG)

A primeira coisa que vamos fazer é criar um servidor local onde vamos fazer nossas requisições. Para isso usamos um método do Express chamado `listen`:

![](/assets/exemplo-img-6.PNG)

Se rodarmos `node index.js` no terminal, e abrirmos `http://localhost:3000` no browser, teremos a mensagem _"Cannot GET /"_. Isso é um bom sinal: significa que agora podemos nos comunicar com o nosso express através do servidor.

![](/assets/exemplo-img-7.PNG)

* **Requisição GET: **A requisição GET faz um pedido ao servidor para que ele mande à nossa aplicação alguma coisa. A razão pela qual nosso localhost nos mostra "Cannot GET /" na página é porque ainda não pedimos nenhuma requisição ao servidor. Com o Express, nós usamos o método get para mediar essa requisição. O método get possui a seguinte sintaxe:

![](/assets/exemplo-img-8.PNG)

> O **caminho **indica o caminho que a nossa requisição GET irá fazer. É a URL que colocarmos depois do "/" no nosso `http://localhost:3000/`... O segundo argumento é a função de **callback**, que diz ao servidor o que fazer quando o caminho é encontrado. Ela precisa de dois argumentos, o **resquest **e o **response.**

![](/assets/exemplo-img-9.PNG)

> Geralmente abreviamos resquest para **req **e response para **res**.

Vamos testar nossa requisição: vamos pedir para o servidor no enviar "Olá Mundo!" quando fizermos a requisição GET:

![](/assets/exemplo-img-10.PNG)

> Se executarmos `node index.js` novamente no nosso terminal, e atualizarmos nossa página no browser, vamos ver a mensagem "Olá Mundo!".
>
> Você já deve ter percebido que toda atualização que fizermos em nosso código, precisamos parar o servidor e executar o `node index.js` novamente para que as mudanças sejam realmente aplicadas. Isso é um processo muito tedioso, e para facilitar, nós vamos usar, a partir de agora uma ferramenta que faz esse trabalho para nós automaticamente: o **Nodemon**.

* Instalando o Nodemon através do terminal

![](/assets/exemplo-img-11.PNG)

A partir de agora, vamos usar o comando `nodemon index.js` para rodar nosso código e deixar que ele atualize automaticamente.

* **Requisição POST: **A requisição POST envia ao servidor a informação que queremos enviar. O método POST no Express possui a mesma sintaxe que o método GET:

![](/assets/exemplo-img-12.PNG)

> Quando enviamos a requisição, enviamos o conteúdo pelo body dela.
>
> Obs.: Perceba aqui que o caminho que utilizamos é o "[http://localhost:3000/usuarios](http://localhost:3000/usuarios)".

![](/assets/exemplo-img-13.PNG)

> O Express não manipula dados enviados com JSON, e então precisamos de uma nova ferramenta chamada Body Parser.:

![](/assets/exemplo-img-15.PNG)

Configuramos o body-parser da seguinte forma:

![](/assets/exemplo-img-16.PNG)

> Lembrando que bodyParser deve ser escrito em \_camelCase \_sempre e deve ficar antes de qualquer utilização do Express!

### Usando o MongoDB

Até agora fizemos requisições GET e POST em nosso servidor, mas não salvamos e nem recuperamos dados de um banco de dados. Precisamos, então, instalar o MongoDB:

![](/assets/exemplo-img-14.PNG)

> Para utilizarmos o Mongo, vamos precisar também de uma ferramenta que permite que utilizemos o Express também no nosso banco de dados, para facilitar ainda mais o código. Essa ferramenta se chama Express-MongoDB. Vamos baixá-la usando o npm:

![](/assets/exemplo-img-17.PNG)

E devemos indicar em nosso `index.js` que utilizaremos o Express-MongoDB:

![](/assets/exemplo-img-18.PNG)

* Linkando nosso banco de dados \(que é hosteado pelo MongoDB em nosso `index.js`\):

![](/assets/exemplo-img-19.PNG)

#### Requisição GET:

Agora vamos utilizar o nosso GET para listar todos os dados que temos em nosso banco de dados:

![](/assets/exemplo-img-20.PNG)

> **Entendendo o código: **Com o MongoDB, conseguimos fazer uma requisição para o nosso banco de dados chamado "meu-bd" na coleção "usuarios". Conseguimos listar todos os documentos que temos em nosso BD através do comando **db.collection\('usuarios'\).find\(\)**.
>
> Porém, o MongoDB nos retorna um objeto \(que é a coleção\) com vários objetos dentro \(que são nossos documentos\). E o JavaScript não consegue interpretar esse tipo de dado. Lembre-se de que sempre que queremos várias informações, precisamos coloca-las em um **vetor**, e é por isso que utilizamos o método **.toArray\(\) **para transformar nossa coleção em um vetor de documentos.
>
> A função **.toArray\(\) **precisa de uma função de callback para nos avisar se foi realmente possível transformar o que nos foi pedido do banco de dados em um vetor. E ela possui a seguinte sintaxe:
>
> ```
> .toArray((erro, resultado) => {
>     if(erro){
>         return erro;
>     } else {
>         return resultados;
>     }
> });
> ```
>
> Caso não seja possível transformar em vetor, ela nos retorna um erro \(err\). Senão, nos retorna o resultado \(result\), que são os documentos escritos em formato de vetor.

### Requisição POST:

![](/assets/exemplo-img-21.PNG)

> **Entendendo o código: **O POST possui uma estrutura muito parecida com a do GET. A única diferença é que ao invés de usarmos o método **.find\(\)**, usamos o método **.insert\(\)**, pois com a requisição POST queremos inserir um novo documento em nossa coleção.
>
> O método insert\(\), assim como o .toArray\(\) que usamos na requisição GET, possui uma função de callback que verifica se foi possível inserir um novo documento na coleção. Caso não foi possível, ela nos retorna um erro. Se foi possível, ela nos retorna um **status code**, que no caso é o "200", que significa "created".

## DESAFIO: Construir um CRUD completo.

Aqui você já aprendeu metade de um CRUD \(Create, Read, Update, Delete\): criamos um novo documento em nossa coleção, e retornamos para nossa aplicação todos os documentos que temos salvos. O desafio é: construir um CRUD completo! Tente você mesmo usar as requisições PUT e DELETE para fazer o UPDATE e o DELETE de itens no banco de dados!



