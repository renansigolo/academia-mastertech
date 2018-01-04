# Desmistificando a Web

Vamos começar a introduzir alguns conceitos básicos para revelar alguns segredos contidos nesse mundo digital.

Aqui você irá encontrar todos os códigos realizados em sala de aula como referência para estudar em casa.

#### Psiuu, da uma olhadinha aqui em algumas dicas que irão te ajudar a ler esta e qualquer outra documentação

* Quando você ver estes 3 pontinhos
  `...`
  normalmente isso indica que você deve substituir eles e preencher com algum outro código.
* Muitas vezes utilizamos os conchetes
  `[ ]`
  para indicar que este parâmetro é opcional.

#### O que é o tal cache?

É onde são armazenados os dados temporários de sua navegação, para agilizar o acesso aos sites visitados anteriormente. Ou seja, imagina que seja uma caixinha que toda vez que você acessa um site é armazenado dados como pesquisa, cliques, no caso de aplicativos, as informações dos aplicativos mais acessados, e cada vez que você acessar um site ou um aplicativo eles vão visitar essa caixinha para que não tenha que fazer do zero, isso ajuda a economizar tempo e tornar a resposta mais rápida.

Porém é comum que alguns dados se misturem ou essa caixinha fique com muita informação. Por isso, é muito comum ouvir apague ou limpe o cache, para elimiar estes dados e ficar mais leve. IMPORTANTE: são dados temporários, dados como senhas salvas, preenchimento automático se mantém.

### Front-end x Back-end

Quem trabalha com front é responsável por toda parte que é visualizada por nós, ou seja cores, botões, cliques, e toda interface do site. Nesta etapa é super importante dar atenção a experiência do usuário, chamado de UX.

O foco principal é em HTML \(linguagem de marcação\), CSS \(linguagem de estilo\) e JavaScript \(linguagem de script/programação\). São linguagens client-side, ou seja do lado do cliente, do usuário do site.

Já quem trabalha com back-end fica na parte de trás, nos bastidores de seu site na parte de implementação, segurança da informação, performance e com banco de dados também.

Em relação as principais linguagens seriam C\#, Java, PHP, Python, Ruby... que seriam algumas das linguagens de programação conhecidas como server-side, que seriam linguagens de servidor que fornece a lógica para cada aplicação. Um exemplo simples, é uma requisição HTTP que seria quando você clica num botão de "cadastrar" e aparece uma página de cadastro e logo em seguida do preenchimento, uma página de cadastro salvo. Todo esse processo de solicitar a página de cadastro, salvar seus dados e receber a confirmação faz parte de uma lógica que é efetuada no back-end.

### Aplicações Móveis

São os nossos conhecidos aplicativos de celular. São desenvolvidos exatamente para ser utilizado no mobile e há opções de aplicações nativas, web app e conhecidas como híbridas.

Aplicações nativas são aquelas desenvolvidas na linguagem do sistema operacional, como por exemplo para IOS que seria a Swift, para Android seria Java e a grande vantagem é se comunicar melhor com os dispositivos do aparelho, como câmera, pedômetro, entre outros. Isso faz com que a aplicação fique mais funcional, com melhor aproveitamento de energia porém geram um conhecimento maior de cada linguagem. A escolha da sua aplicação depende muito da sua necessidade e do seu negócio.

Uma solução muito utilizada é o Ionic que é um framework para desenvolvimento de aplicações híbridas para dispositivos móveis de rápido e fácil desenvolvimento.

### O que é uma API

A sigla significa "Application Programming Interface" que funciona para criar uma interface \(caminho\) com regras bem definidas para integração entre aplicações, para troca de informações e para trabalhar com elas.

De forma mais simples, é o que acontece com alguns sites que possuem mapas de localização, o Google fornece uma parte de seu código utilizado na criação do aplicativo Google Maps, e isso é incorporado no site. Quando por exemplo você clica em um endereço de uma loja e aparece a rua e a localização em um mapa, significa que a sua requisição chegou no Google e ele respondeu mostrando o local no mapa.

Um outro bom exemplo é uma rede social como o Facebook, que foram criadas diversas APIs que possibilitaram receber informações de uma conta ou mesmo em fazer login em outros sites, utilizando uma conta do Facebook.

#### O que é Node.js?

É uma plataforma que lê e entende o Javascript pelo lado do browser e também do servidor. Isso torna o processo muito mais ágil. Mas como assim?

Imagine que você tem um site e seu usuário vai fazer o login, ele vai inserir o email e a senha, ou seja, acontecerá uma requisição para o banco de dados para validar e liberar o acesso a outra página. Porém, ao invés de aguardar esta resposta do banco, ele já antecipa a próxima requisição e quando ele receber a resposta é enviado o evento sem deixar as demais requisições paradas e sem sobrecarregar o servidor. O processamento de requisições é muito mais alto e rápido. Por exemplo, um site que utiliza é o Walmart. Imagina na black friday que são milhares de acessos e requisições \(compra, cadastro, pagamento...\) se não tiver um processamento rápido, poderiam perder muitas vendas.

Instalando o NodeJS  - [https://nodejs.org/en/](https://nodejs.org/en/)

A versão mais recente e recomendada para a maioria dos usuarios  é a 8.9.1 LTS.

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

