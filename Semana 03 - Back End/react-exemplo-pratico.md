# React - Exemplo Prático

Com nosso aplicativo default criado, abra o código com sua IDE de preferência.

Dentro da pasta _**./src **_é onde vamos fazer começar nossa aplicação, crie uma nova pasta chamada _**./component **\_para abrigar os componentes que vamos usar em nosso site, e uma pasta chamada _**./assets **\_para conter os arquivos de imagens e outros.

O primeiro componente que vamos criar será o  **Header**, dentro dele ira ter o navbar  e um menu lateral quando clicarmos na navbar e o um banner passando imagens.

* Crie arquivo _**Header.js **\_e _**Header.css**_, dentro da pasta  **.**_**/component**\_, na class nav usaremos transform e transition para estilizar o menu lateral com eixo X -100% para esconder, e na class nav .ativa alteramos o eixo X para 0% para exibi-la.

  ![](/assets/cssreact.png)

* Além da importação do React, importe o Header.css. Devemos usar uma propriedade nativa do React chamada _**componentWillMount\(\) **_e_** setState\(\) **_com a 1ª propriedade configuramos para que o método randerize antes da página ser exibida, a 2ª propriedade permite que possamos 

![](/assets/headerjs.png)



