# Back-End: Teoria

![](/assets/back.png)

Quando o usuário digita um endereço, é o back-end que processa aquele endereço e envia os dados para o front-end apresentar na tela.Por ser uma área muito abrangente, existem diversas linguagens, frameworks e tecnologias. Cada um deles é focado em diferentes aspectos e soluções. Existem as tecnologias de back-end voltadas para web, como:

PHP

Ruby on Rails

Node.js

Python

E existem também as linguagens focadas em soluções desktop, os famosos programas de computadores e sistemas:

C

C\#

C++

Java

## Cliente x Servidor

A Internet é uma rede de computadores interligados em escala mundial. A cada dia, mais e mais computadores são conectados a Internet, e ela fica cada vez mais extensa. Surgiu então, a necessidade de dedicar computadores especialmente para prover serviços à rede, enquanto os demais usufruem dessa rede. Esses computadores especiais são chamados de **Servidores**, enquanto os computadores normais \(como os nossos que usamos para escrever códigos\) são chamados de **Clientes**. É por isso que falamos que o HTML, por exemplo, executa no _client-side,_ e quando queremos pegar algum dado que está em um banco de dados, esse processo é execudado no _server-side_.

Toda vez que um Cliente pede uma requisição ao servidor, essa requisição é encaminhada através da Internet. Por exemplo, quando queremos entrar no site do _Google_, fazemos uma **requisição** para o servidor onde o site _google.com.br_ está sendo hospedado. Quando nosso computador faz essa requisição, ela é transmitida até o servidor do _Google_ passando por vários servidores até chegar no específico. E quando chega, a requisição se transforma em uma resposta \(que no nosso exemplo é o endereço do site do _Google_\), e é enviada de volta para o cliente.

## Protocolo HTTP

O nome parece complicado mas é só uma sigla, que vem de _HyperText Transfer Protocol_. Mas o que é isso, afinal?

Basicamente é um protocolo que permite enviar e receber informações na web. E o que é um protocolo?

Um protocolo é um conjunto de regras que determinam que tipo de informações podem ser trocadas e que tipo de mensagem deve ser enviada.

O Protocolo HTTP precisa do cliente e do servidor para funcionar corretamente. Convencionalmente os pedidos são chamados de _**request**_ e as respostas de _**response**_. Todos os \_requests \_e \_responses \_que fazemos para um servidor possui junto com a informação que queremos enviar/receber um protocolo. Existem vários tipos de protocolos, e o mais usual deles é o HTTP. Conheça mais tipos [aqui](https://www.weblink.com.br/blog/tecnologia/conheca-os-principais-protocolos-de-internet/ "Principais protocolos de Internet"). ![](/assets/http.png)

#### Requisições HTTP

Quando estamos navegando na internet, a todo momento o nosso navegador está enviando requisições para um servidor e o servidor, por sua vez, nos devolve uma resposta em um formato específico ou realiza uma ação de acordo com o que pedirmos para ele fazer. Isso ocorre diversas vezes como por exemplo ao preencher um formulário, fazer um login, acessar suas matérias online da faculdade...

Por exemplo, quando acessamos a ferramenta Inspect, e ir na aba Network conseguimos ver todo esse processo a cada vez que carregamos um site:![](/assets/http01.png)

### Principais métodos de requisições

O protocolo HTTP define uma série de métodos de requisição \(request methods\) responsáveis por indicar a ação a ser executada sob o dado que estamos enviando ou recebendo do servidor. São os mais importantes:

* **GET:**  Essa é a requisição mais comum de todas. Através dessa requisição nós pedimos as informações do servidor, que pode ser um arquivo HTML, XML, JSON, etc.

* **POST:**  O método POST é utilizado quando queremos criar um recurso. Um bom exemplo é quando temos um formulário. Quando clicamos em uma aba "contato" é um GET, mas quando inserimos dados e clicamos no enviar este seria um POST. Ele cria, adiciona e envia ao servidor.

* **PUT**:  Quando um recurso precisa ser atualizado e ele já existe, já esta dentro do servidor. Se não existir, pode ser criado. Por exemplo, quando você faz uma atualização de cadastro ou quando você já tem um cadastro e é solicitado mais um número de telefone para contato. Você já existe dentro do servidor mas pode atualizar ou criar algo novo.

* **DELETE:**  Como a palavra diz, é uma requisição para excluir o recurso especificado. Por exemplo, quando você apaga um conta do twitter, ou o dado de um cartão salvo em um e-commerce.

![](/assets/codes-status.png)

### HTTP x HTTPS

Porque algumas vezes, quando estamos usando o nosso browser, ele usa o HTTPS ao invés de HTTP?

HTTPS significa _**HyperText Transfer Protocol Secure**_. Usando esse tipo de protocolo, o cliente avisa ao servidor que os dados que ele enviará são, por exemplo, **sigilosos**, e que devem ser codificados para serem enviados. Dessa forma, quando os dados são enviados, eles estão todos embaralhados, e só conseguem ser decodificados pelo servidor no qual queremos que os dados cheguem. A "chave" para decodificar os dados está escrita no HTTPS, e é lida somente pelo servidor. Isso mantém suas informações seguras de hackers, por exemplo.

Um exemplo de sites que utilizam o protocolo HTTPS são os sites de bancos, ou qualquer site que utilizem senhas para entrar!

### IP

IP \(_Internet Protocol_\) é uma sequência de protocolos que representa as regras de comunicação da _Internet, \_e baseia-se no endereçamento \_IP:porta_ para cada cliente que está conectado à rede de _Internet_. O endereço IP serve para identificar, de maneira única, um computador na rede, já a porta indica por onde e quais dados entrarão no computador-cliente.

Uma boa metáfora para entender IP:Porta é a seguinte: imagine que o cliente mora em um prédio em um dado endereço, num apartamento X. O IP do cliente é o endereço do prédio, e a sua porta X é o número de seu apartamento.

A combinação IP + porta se chama _**socket**_. O número de porta para quando enviamos arquivos HTTP é a de número 80, e a de HTTPS é a 443. Descubra [aqui](http://www.meuip.com.br/) qual é o IP do seu computador!

#### O que é NPM?

A NPM \(_Node Package Manager_\) é duas coisas: primeiro, é um repositório online para publicação de projetos de código aberto para o Node.js e além disso ele é uma linha de comando que interage com este repositório online, que ajuda na instalação de pacotes, gerenciamento de versão e gerenciamento de dependências, tudo feito via terminal.

#### O que é Node.js?

É uma plataforma que lê e entende o Javascript pelo lado do browser e também do servidor, assim é possível  usar a mesma biblioteca, objetos iguais e ter melhor controle sobre o código. Isso torna o processo muito mais ágil. Mas como assim?

Imagine que você tem um site e seu usuário vai fazer o login, ele vai inserir o email e a senha, e fará uma requisição para o banco de dados para validar e liberar o acesso a outra página. Porém, ao invés de aguardar esta resposta do banco, ele já antecipa as próximas requisições, e quando o site receber a resposta daquela primeira requisição, a validação é recebida sem deixar as demais paradas e sem sobrecarregar o servidor. O processamento de requisições é muito mais alto e rápido. Por exemplo, um site que utiliza é o Walmart. Imagine que na _black friday_ são milhares de acessos e requisições \(compra, cadastro, pagamento...\) se não tiver um processamento rápido, poderiam perder muitas vendas.

Instalando o NodeJS  - [https://nodejs.org/en/](https://nodejs.org/en/)

#### **Database**

A database ou banco de dados funciona como uma biblioteca repleta de informações, o cérebro que faz os sites serem dinâmicos. Toda vez que você realiza uma ação ou procura algo em um site, a database é responsável por aceitar sua busca, encontrar o dado e apresentar no website. No back-end, a database é acessada pelos usuários indiretamente a partir de uma aplicação externa. Alguns exemplos são MySQL, MongoDB, Postgresql e NoSQL.

**API**

Uma API  é que uma interface que permite que dois sistemas, ainda que criados com tecnologias diferentes, se comuniquem através de uma linguagem comum. Elas conectam softwares, aplicações, databases e serviços, substituindo a necessidade de uma programação mais complexa. Por exemplo o Waze está conectado ao Spotify, então assim autoriza a integração, você faz o contato com Spotify para navegar, e assim que fizer a "chamada" para ouvir a playlist, ela vai buscar esta lista e começar o streaming, é este processo que chamamos de integração.

**Escalabilidade**

A tecnologia continua mudando, os modelos de negócio mudam e o sistema de back-end precisa ser construído de forma a se adaptar facilmente à essas mudanças. É para isso que serve a escalabilidade, um dos conceitos mais importantes no back-end. É preciso pensar em quão flexível é a estrutura de uma aplicação para acomodar novos códigos, mais tráfego e dados.

