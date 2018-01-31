# IONIC 1

## O que é IONIC?

Assim como o Bootstrap é um framework para auxiliar na criação do CSS o IONIC é um framework para nos ajudar a criar uma aplicação mobile que será convertida para um aplicativo iOS e/ou Android.

Com o Ionic é possível escrever código uma única vez e ter um aplicativo que roda ‘nativamente’ \(entre aspas pois não é totalmente nativo\) no iPhone, Android e Windows Phone. Isso é possível pois estes Sistemas Operacionais Móveis possuem APIs \(_Application Program Interface_\) usadas para que seus programadores desenvolvam aplicativos nativos para a plataforma.

Para ser mais claro, você irá construir um aplicativo para iOS e Android utilizando linguagens de programação Web, sem precisar aprender Swift ou Kotlin.

O que o Ionic faz é, através do Apache Cordova, se comunicar com estas APIs que, por sua vez, comunica-se com um componente chamado Web View, usado por aplicativos nativos para visualização de páginas web dentro do contexto dos aplicativos móveis\(como um Browser qualquer\). O Ionic permite que nosso aplicativo rode embarcado dentro dessa Web View,

O Ionic permite que nosso aplicativo rode, interprete e renderize o código HTML, CSS e JavaScript do aplicativo. O Ionic também estiliza o componentes HTML para se parecer com os componentes nativos de cada plataforma móvel, simulando a experiência nativa do usuário final.

### Ionic Framework

O ionic framework é toda a estrutura, comandos etc que irá suportar seu app.

Como o Ionic foi criado em cima do Angular ele também é dividido em duas partes

* [**Ionic 1**](https://ionicframework.com/docs/v1/)

  * Toda a estrutura do Ionic 1 utiliza o AngularJS como padrão

* [**Ionic 2/3**](https://ionicframework.com/framework)

  * A partir da segunda versão do Ionic ele já utiliza o novo Angular, atualmente chamado apenas de Angular que é escrito em Typescript e o Cordova para criar nosso código nativo!

Neste curso vamos utilizar somente o Ionic 3, mas é importante que você saiba as diferenças para não se confundir na hora de escrever seu código ;\)

# Meu primeiro App em Ionic

Borá aprender como iniciar nosso primeiro app então!

### Criando nossa primeira aplicação \(CLI\)

Para iniciar seu primeiro app siga as instruções na página [Getting Started](https://ionicframework.com/getting-started/) do Ionic

### Documentação

Para nos auxiliar no desenvolvimento o Ionic possui uma extensiva [documentação](https://ionicframework.com/docs/) que irá nos auxiliar na hora de criar nosso app.

**Pré-requisitos:**

**NodeJS**

**NPM**

Primeiros passos

```
npm install -g cordova ionic

ionic start "seunomedoApp" tabs

//se quiser utilizar a versão 1, basta colocar:
ionic start "seunomedoApp" tabs --type ionic1

//para rodar basta colocar, acesse a pasta do seu projeto Ionic
ionic serve

//para começar a mexer nos templates acessar a pasta www e dentro dela a pasta templates.
```

![](/assets/2018-01-31.png)

##### Como estilizar o seu CSS do Ionic

Da mesma forma que podemos trabalhar o CSS no html, no ionic é a mesma coisa, mudando apenas as tags utilizadas em cada página. Um exemplo seria desta forma:

```
  //html
  <ion-list>  
        <ion-item>

           <a class="item item-avatar" href="#">
              <img ng-src="{{x.Image}}">
              <h2>{{x.Name}}</h2>
              <p id="texto">  {{x.Local}}</p>
            </a>

        </ion-item>
    </ion-list> 

    //css
ion-list ion-item {
  background: green;
}

.item-avatar {
  background: red;
  color: #FFF;
  padding:20px;
}

#texto{
text-align: center;
}
```



