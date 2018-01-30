# AngularJS

AngularJS é um framework de JavaScript que dá suporte na criação de _single-page applications_. Sua implementação é baseada na arquitetura MVC \(_Model-View-Controler_\), que separa a manipulação de dados do HTML de sua visualização estática. O AngularJS funciona por meio da leitura do HTML da aplicação, que tem embutido em suas tags atributos adicionais personalizados, chamados diretivas. O framework interpreta esses atributos para ligar partes da entrada ou saída da página para um modelo que é representado por variáveis no script.

### Single-page application \(SPA\)

Um "aplicativo de página única", ou em inglês _single-page application_, são aplicações completas, desenvolvidas em JavaScript, que funcionam quase como se estivessem sendo executadas nativamente no desktop. As aplicações e os sites SPA, fazem uma transição entre os _templates_ carregados, sem _reload_ de página e sem que o usuário viaje de uma página para outra.

As vantagens de se utilizar SPA, segundo o site [locaweb](http://blog.locaweb.com.br/artigos/desenvolvimento-artigos/o-que-e-single-page-application/), são:

> **1. Melhor experiência do usuário:**
>
> O usuário tem uma experiência melhor navegando no sistema, dando a impressão até de que é um sistema desktop, já que não possui refreshs na página. Dependendo do sistema ele é capaz de funcionar mesmo se o usuário perder a conexão com a Internet. Aqui podemos também fazer uma comparação com apps mobile, já que os apps híbridos são SPA. O que faz com que o usuário que acessa uma SPA pelo celular tem a impressão de estar usando um app e não acessando um site no navegador.
>
> **2. Performance:**
>
> O sistema fica muito mais performático, por que ele carrega o sistema completo na primeira requisição de forma assíncrona que permite o usuário já consumir o  conteúdo sem esperar que tudo seja carregado por completo e as requisições seguintes são responsáveis por trafegar apenas os dados brutos entre o cliente e o servidor, normalmente no formato JSON.
>
> **3. Responsabilidade do client-side:**
>
> Nas SPA o lado cliente ganha mais responsabilidade, já que delegamos lógica ao seu lado e isso acaba ajudando a performance também, dado que o tempo de requisição diminui bastante.
>
> **4. Facilidade de manutenção:**
>
> Quando trabalhamos com SPA deixamos  muito bem separado as partes do que é front-end e o que é back-end, já que todo o back costuma estar em uma API, assim podemos fazer mudanças em back sem precisar mexer em nada de front e vice versa.

### Arquitetura MVC \(Model-View-Controller\)

O MVC é uma arquitetura \(padrão para se escrever o código\) que separa a aplicação em três camadas: a visão \(view\), o modelo \(model\), e o controlador \(controller\).

![](/assets/arquitetura_mvc.png)

* **A camada View:** 
  * É a camada que exibe os dados \(interface do usuário\);
  * Usualmente é montada com HTML e CSS;
  * É responsável por utilizar as informações modeladas \(transformadas em algo útil para o usuário pelo JavaScript\) para produzir interfaces de apresentação conforme a necessidade.

![](/assets/view_exemplo.PNG)

* **A camada Model:**
  * É a camada que contém a estrutura do dado por trás de uma parte específica da aplicação;
  * Responsável pela leitura, manipulação e validação de dados;
  * Obtém os dados e os traduz em informações relevantes para serem exibidas pela View;
  * Notifica a View e o Controller associados, quando há uma mudança em seu estado.

![](/assets/model_exemplo.png)

* **A camada Controller:**
  * Exerce o controle de qual Model deverá ser aplicada e qual View será mostrado ao usuário.
  * O Controller manipula e roteia as requisições dos usuários;
  * Interpreta as requisições submetidas pelo usuário e traduz em comandos que são enviados para o Model e/ou para a View;

![](/assets/controller_exemplo.PNG)



### Diretivas

Angular Básico

Documentação oficial: [https://angularjs.org/](https://angularjs.org/)

* Arquitetura do Angular: [https://angular.io/guide/architecture](https://angular.io/guide/architecture)
* Módulos
* Criar e utilizar componentes
* Diretivas: ngFor
* Eventos: click

## Angular CLI

Programa de terminal que cria e gerencia aplicações Angular

### Referência de comandos

* Instala o Angular CLI

  `npm install -g @angular/cli`

* Inicia um projeto

  `ng new NomeDoProjeto`

* Inicia o ambiente de desenvolvimento

  `ng serve`

* Cria um Componente

  `ng generate component NomeDoComponente`

* Cria um serviço

`ng generate service NomeDoServico`

Serviços e comunicação entre componentes:

[https://angular.io/guide/component-interaction\#parent-and-children-communicate-via-a-service](https://angular.io/guide/component-interaction#parent-and-children-communicate-via-a-service)

