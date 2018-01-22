# BACK-END

![](/assets/back.png)

## Cliente x Servidor

A Internet é uma rede de computadores interligados em escala mundial. A cada dia, mais e mais computadores são conectados a Internet, e ela fica cada vez mais extensa. Surgiu então, a necessidade de dedicar computadores especialmente para prover serviços à rede, enquanto os demais usufruem dessa rede. Esses computadores especiais são chamados de **Servidores**, enquanto os computadores normais \(como os nossos que usamos para escrever códigos\) são chamados de **Clientes**. É por isso que falamos que o HTML, por exemplo, executa no _client-side,_ e quando queremos pegar algum dado que está em um banco de dados, esse processo é execudado no _server-side_.

Toda vez que um Cliente pede uma requisição ao servidor, essa requisição é encaminhada através da Internet. Por exemplo, quando queremos entrar no site do _Google_, fazemos uma **requisição** para o servidor onde o site _google.com.br \_está sendo **hospedado**. Quando nosso computador faz essa requisição, ela é transmitida até o servidor da \_Google_ passando por vários servidores até chegar no específico. E quando chega, a requisição se transforma em uma **resposta **\(que no nosso exemplo é o endereço do site do _Google_\), e é enviada de volta para o cliente.

## Protocolo HTTP

O nome parece complicado mas é só uma sigla, que vem de _HyperText Transfer Protocol_. Mas o que é isso, afinal?

Basicamente é um protocolo que permite enviar e receber informações na web. E o que é um protocolo?

Um protocolo é um conjunto de regras que determinam que tipo de informações podem ser trocadas e que tipo de mensagem deve ser enviada.

O Protocolo HTTP precisa do cliente e do servidor para funcionar corretamente. Convencionalmente os pedidos são chamados de _**request**_ e as respostas de _**response**_. Todos os \_requests \_e \_responses \_que fazemos para um servidor possui junto com a informação que queremos enviar/receber um protocolo. Existem vários tipos de protocolos, e o mais usual deles é o HTTP. Conheça mais tipos [aqui](https://www.weblink.com.br/blog/tecnologia/conheca-os-principais-protocolos-de-internet/ "Principais protocolos de Internet"). ![](/assets/http.png)

#### Requisições HTTP

Quando estamos navegando na internet, a todo momento o nosso navegador está enviando requisições para um servidor e o servidor, por sua vez, nos devolve uma resposta em um formato específico ou realiza uma ação de acordo com o que pedirmos para ele fazer. Isso ocorre diversas vezes como por exemplo ao preencher um formulário, fazer um login, acessar suas matérias online da faculdade...

Por exemplo, quando acessamos a ferramenta Inspect, e ir na aba Network conseguimos ver todo esse processo a cada vez que carregamos um site:![](/assets/http01.png)

O _**Request Method**_ indica quais o nosso objetivo quando fazemos uma requisição ao servidor, por exemplo, pegar informações do servidor.

##### Principais métodos:

GET:  
 Essa é a requisição mais comum de todas. Através dessa requisição nós pedimos as informações do servidor, que pode ser um arquivo HTML, XML, JSON, etc.

POST:  
 O método POST é utilizado quando queremos criar um recurso. Um bom exemplo é quando temos um formulário. Quando clicamos em uma aba "contato" é um GET, mas quando inserimos dados e clicamos no enviar este seria um POST. Ele cria, adiciona e envia ao servidor.

PUT:  
 Quando um recurso precisa ser atualizado e ele já existe, já esta dentro do servidor. Se não existir, pode ser criado. Por exemplo, quando você faz uma atualização de cadastro ou quando você já tem um cadastro e é solicitado mais um número de telefone para contato. Você já existe dentro do servidor mas pode atualizar ou criar algo novo.

DELETE:  
 Como a palavra diz, é uma requisição para excluir o recurso especificado. Por exemplo, quando você apaga um conta do twitter, ou o dado de um cartão salvo em um e-commerce.

### HTTP x HTTPS

Porque algumas vezes, quando estamos usando o nosso browser, ele usa o HTTPS ao invés de HTTP?

HTTPS significa _**HyperText Transfer Protocol Secure**_. Usando esse tipo de protocolo, o cliente avisa ao servidor que os dados que ele enviará são, por exemplo, **sigilosos**, e que devem ser codificados para serem enviados. Dessa forma, quando os dados são enviados, eles estão todos embaralhados, e só conseguem ser decodificados pelo servidor no qual queremos que os dados cheguem. A "chave" para decodificar os dados está escrita no HTTPS, e é lida somente pelo servidor. Isso mantém suas informações seguras de hackers, por exemplo.

Um exemplo de sites que utilizam o protocolo HTTPS são os sites de bancos, ou qualquer site que utilizem senhas para entrar!

### IP

IP \(_Internet Protocol_\) é uma sequência de protocolos que representa as regras de comunicação da _Internet, \_e baseia-se no endereçamento \_IP:porta_ para cada cliente que está conectado à rede de _Internet_. O endereço IP serve para identificar, de maneira única, um computador na rede, já a porta indica por onde e quais dados entrarão no computador-cliente.

Uma boa metáfora para entender IP:Porta é a seguinte: imagine que o cliente mora em um prédio em um dado endereço, num apartamento X. O IP do cliente é o endereço do prédio, e a sua porta X é o número de seu apartamento.

A combinação IP + porta se chama _**socket**_. O número de porta para quando enviamos arquivos HTTP é a de número 80, e a de HTTPS é a 443. Descubra [aqui](http://www.meuip.com.br/) qual é o IP do seu computador!

### Sintaxe de um Protocolo HTTP

Existem duas coisas bem importantes em uma mensagem HTTP:

* **Header**

  * Contém as instruções para a transferência das informações que estão contidas no _body_ e até métodos HTTP.

* **Body**

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

### Query Strings

Tudo o que vem depois da "?" é o que chamamos de query string, que são informações que serão interpretadas pela aplicação que é executada no servidor.

![](/assets/tag.jpg)

#### O que é URI?

Um URI \(do inglês Uniform Resource Identifier\) são vários caracteres usados para identificar ou denominar uma aplicação na internet para interagir com representações desta aplicação por intermédio da internet. Um bom exemplo é a URL.

#### O que é NPM?

A NPM é duas coisas: primeiro, é um repositório online para publicação de projetos de código aberto para o node.j e além disso ele é uma linha de comando que interage com este repositório online, que ajuda na instalação de pacotes, gerenciamento de versão e gerenciamento de dependências, tudo feito via terminal.

#### O que é Node.js?

É uma plataforma que lê e entende o Javascript pelo lado do browser e também do servidor. Isso torna o processo muito mais ágil. Mas como assim?

Imagine que você tem um site e seu usuário vai fazer o login, ele vai inserir o email e a senha, e fará uma requisição para o banco de dados para validar e liberar o acesso a outra página. Porém, ao invés de aguardar esta resposta do banco, ele já antecipa as próximas requisições, e quando o site receber a resposta daquela primeira requisição, a validação é recebida sem deixar as demais requisições paradas e sem sobrecarregar o servidor. O processamento de requisições é muito mais alto e rápido. Por exemplo, um site que utiliza é o Walmart. Imagine que na black friday são milhares de acessos e requisições \(compra, cadastro, pagamento...\) se não tiver um processamento rápido, poderiam perder muitas vendas.

Instalando o NodeJS  - [https://nodejs.org/en/](https://nodejs.org/en/)

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

