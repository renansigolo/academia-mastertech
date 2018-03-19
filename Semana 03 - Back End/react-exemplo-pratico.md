# React - Exemplo Prático

Com nosso aplicativo default criado, abra o código com sua IDE de preferência.

Dentro da pasta _**./src **_é onde vamos começar nossa aplicação, crie uma nova pasta chamada _**./component **\_para abrigar os componentes que vamos usar em nosso site, e uma pasta chamada _**./assets **\_para conter os arquivos de imagens e outros.

O primeiro componente que vamos criar será o  **Header**, dentro dele ira ter o navbar  e um menu lateral quando clicarmos na navbar e o um banner passando imagens.

* Crie arquivo _**Header.js **\_e _**Header.css**_, dentro da pasta  **.**_**/component**\_, na class nav usaremos transform e transition para estilizar o menu lateral com eixo X -100% para esconder, e na class nav .ativa alteramos o eixo X para 0% para exibi-la.

  ![](/assets/cssreact.png)

* Além da importação do React, importe o Header.css. Devemos usar uma propriedade nativa do React chamada \_**componentWillMount\(\) **\_e** setState\(\), ** a 1ª propriedade configuramos para que o método randerize antes da página ser exibida, a 2ª propriedade permite que possamos alterá-la como objeto.

* _**className={}** _ no html permite alterar classe do css apra exibir o menu lateral e ocultá-lo.

![](/assets/headerjs.png)

* Importe o \_**&lt;Header /&gt; **\_para o arquivo** App.js**.

![](/assets/sidemenu.png)

* Crie o componente  \_**Banner.js **\_importamos as 3 imagens dentro de um vetor global usando um **for\(\){} **para percorrer e exibi-la com a propriedade componentWillMount, dentro dele setInterval\(\), para alternar em 2s.

![](/assets/banner.png)

* Crie o componente **Lista.js **nele irá conter uma lista opções do cardápio.
* Crie um arquivo chamado **produtos.json** será os pratos da lista.

![](/assets/json.png)

* Importe os nossos produtos para a Lista.js 
  * Usaremos um for\(\){} para por cada objeto do vetor de produtos

![](/assets/listaJs.png)

* Importe \_**&lt;Lista/&gt;** \_para o App.js.

![](/assets/appJs.png)

* Inicie o spa.

```
$ npm start
```



clique para ver o [**código**](https://github.com/estacaohack3/403-restaurante).



