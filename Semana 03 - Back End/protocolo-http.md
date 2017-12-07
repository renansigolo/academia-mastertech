# Protocolo HTTP - Caique

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

### O que são os métodos HTTP?

* **GET**
  * Mussum Ipsum, cacilds vidis litro abertis. Copo furadis é disculpa de bebadis, arcu quam euismod magna. Nec orci ornare consequat. Praesent lacinia ultrices consectetur. Sed non ipsum felis. Tá deprimidis, eu conheço uma cachacis que pode alegrar sua vidis. Quem manda na minha terra sou euzis!
* **POST**
  * Mussum Ipsum, cacilds vidis litro abertis. Copo furadis é disculpa de bebadis, arcu quam euismod magna. Nec orci ornare consequat. Praesent lacinia ultrices consectetur. Sed non ipsum felis. Tá deprimidis, eu conheço uma cachacis que pode alegrar sua vidis. Quem manda na minha terra sou euzis!
* **PUT**
  * Mussum Ipsum, cacilds vidis litro abertis. Copo furadis é disculpa de bebadis, arcu quam euismod magna. Nec orci ornare consequat. Praesent lacinia ultrices consectetur. Sed non ipsum felis. Tá deprimidis, eu conheço uma cachacis que pode alegrar sua vidis. Quem manda na minha terra sou euzis!
* **DELETE**
  * Mussum Ipsum, cacilds vidis litro abertis. Copo furadis é disculpa de bebadis, arcu quam euismod magna. Nec orci ornare consequat. Praesent lacinia ultrices consectetur. Sed non ipsum felis. Tá deprimidis, eu conheço uma cachacis que pode alegrar sua vidis. Quem manda na minha terra sou euzis!
* asdasd



