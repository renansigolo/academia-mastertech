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

Se executarmos `node index.js` novamente no nosso terminal, e atualizarmos nossa página no browser, vamos ver a mensagem "Olá Mundo!".

