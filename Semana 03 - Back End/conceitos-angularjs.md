# AngularJS - Services e Factory

Os serviços AngularJS são objetos substituíveis que são conectados juntos usando [injeção de dependência \(DI\)](https://docs.angularjs.org/guide/di).Você pode usar serviços para organizar e compartilhar código em seu aplicativo.

Os serviços AngularJS são:

* Instantivamente instanciado - AngularJS apenas instancia um serviço quando um componente de aplicativo depende disso.
* Singletons - Cada componente dependente de um serviço obtém uma referência à única instância gerada pela fábrica de serviços.

## Criando Serviços {#creating-services}

Os desenvolvedores de aplicativos são livres para definir seus próprios serviços registrando o nome do**serviço**e a**função de fábrica do serviço**, com um módulo AngularJS.

A **função de fábrica do serviço **gera o único objeto ou função que representa o serviço para o resto do aplicativo.O objeto ou função retornada pelo serviço é injetado em qualquer componente \(controlador, serviço, filtro ou diretiva\) que especifica uma dependência no serviço.

