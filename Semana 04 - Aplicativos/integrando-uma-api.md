# Protocolo HTTP

O nome parece complicado mas é só uma sigla, que vem de _HyperText Transfer Protocol_. Mas o que é isso, afinal?

Basicamente é um protocolo que permite enviar e receber informações na web. E o que é um protocolo?

Um protocolo é um conjunto de regras que determinam que tipo de informações podem ser trocadas e que tipo de mensagem deve ser enviada.

O Protocolo HTTP precisa de duas entidades para funcionar corretamente: o **cliente** e o **servidor**. E normalmente o cliente é quem inicia a conversa e o servidor responde, criando uma linha de comunicação entre eles. Convencionalmente os pedidos são chamados de _**request**_ e as respostas de _**response**_.![](/assets/http.png)Existem duas coisas bem importantes em uma mensagem HTTP:

* **Header**

  * Pode conter instruções para a transferência das informações do body e até métodos HTTP.

* **Body**

  * Pode estar vazio ou conter informações que você deseja transmitir através da rede.

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

### Requisições HHTP

Quando estamos navegando na internet, a todo momento o nosso navegador está enviando requisições para um servidor e o servidor, por sua vez, nos devolve uma resposta em um formato específico ou realiza uma ação de acordo com o que pedirmos para ele fazer. Isso ocorre diversas vezes como por exemplo ao preencher um formulário, fazer um login, acessar suas matérias online da faculdade...

Por exemplo, quando acessamos a ferramenta Inspect, e ir na aba Network conseguimos ver todo esse processo a cada vez que carregamos um site:![](/assets/http01.png)

#### O Request Method indica quais o nosso objetivo quando fazemos uma requisição ao servidor, por exemplo, pegar informações do servidor.

##### Principais métodos:

GET : Essa é a requisição mais comum de todas. Através dessa requisição nós pedimos as informações do servidor, que pode ser um arquivo html, xml, json, etc. 

POST : O método POST é utilizado quando queremos criar um recurso. Um bom exemplo é quando temos um formulário. Quando clicamos em uma aba "contato" é um GET, mas quando inserimos dados e clicamos no enviar este seria um POST. Ele cria, adiciona e envia ao servidor.

PUT : Quando um recurso precisa ser atualizado e ele já existe, já esta dentro do servidor. Se não existir, pode ser criado. Por exemplo, quando você faz uma atualização de cadastro ou quando você já tem um cadastro e é solicitado mais um número de telefone para contato. Você já existe dentro do servidor mas pode atualizar ou criar algo novo.

DELETE : Como a palavra diz, é uma requisição para excluir o recurso especificado. Por exemplo, quando você apaga um conta do twitter, ou o dado de um cartão salvo em um e-commerce.

### API's

API é uma forma de integrar um sistema no outro. Por exemplo o Waze está conectado ao Spotify, então assim autoriza a integração, você o contato com Spotify para navegar, e assim que fizer a "chamada" para ouvir a playlist, ela vai buscar esta lista e começar o streaming, é este processo que chamamos de integração.





