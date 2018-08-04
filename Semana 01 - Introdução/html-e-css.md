# HTML e CSS

É hora de por a mão na massa e começar a mexer em códigos!

## HTML

HTML é o corpo do seu site, toda a estrutura da página é feito por html. Ele faz o posicionamento de cada item seja título, parágrafo, imagem ou um link. Ele é formado por tags como por exemplo &lt;body&gt; e toda tag deve ser fechada no seu código.

##### ![](/assets/code1.png)

## Tags mais utilizadas no HTML

* `<p>Paragrafo</p>`

* `<h1>Título</h1>`

* `<ul>Lista</ul>`

* `<li>Item da lista</li>`

* `<img src="endereco-da-imagem">`

* `<section> ... <section>`

* `<footer> ... </footer>`

### Form

* Tag de formulário

`<form> </form>`

* Tag do campo de inserção

`<input> <input placeholder="Digite seu nome...">`

* Botão

`<button type="button">Enviar</button>`

### Formulário Completo

```
  <section>
    <form action="/" method="post">
      <input type="text" name="name" placeholder="Digite aqui seu Nome">
      <input type="email" name="email" placeholder="Digite aqui seu Email">
      <input type="password" name="pass" placeholder="Digite aqui sua Senha">
      <button type="button" name="button">Clique aqui para Logar</button>
    </form>
  </section>
```

![](/assets/Screen Shot 2017-11-16 at 3.37.31 pm.png)

### Head

* Exemplo de cabeçalho

```
<head>
    <meta charset="utf-8">
    <title>Nome da Aba do Navegador</title>
    <link rel="stylesheet" href="styles.css">
</head>
```

### Partes essenciais no HTML

&lt;!DOCTYPE html&gt; — o doctypegera que os navegadores que não oferecem suporte ao HTML5 interpretarão as partes já estabelecidas pelo HTML em um modo "compatível" com HTML5, ignorando as funcionalidades que ele não suporta.

&lt;html&gt;&lt;/html&gt; — o elemento &lt;html&gt;. Esse elemento envolve todo o conteúdo da página, é o elemento raiz, a tudo que terá em seu site estará dentro desta tag.

&lt;head&gt;&lt;/head&gt; — o elemento &lt;head&gt;. Esse elemento age como um recipiente de tudo o que você deseja incluir em uma página HTML que não é o conteúdo que você quer mostrar para quem vê sua página. Isso inclui coisas como CSS para dar estilo ao conteúdo, links incorporados de fontes, palavras-chaves para SEO e mais.

&lt;body&gt;&lt;/body&gt; — o elemento &lt;body&gt;. Contém todo o conteúdo que você quer mostrar ao público que visita sua página, seja texto, imagens, vídeos, jogos, formulários…

&lt;meta charset="utf-8"&gt; — esse elemento aponta qual conjunto de caracteres seu documento deve usar para o utf-8, que inclui praticamente todos os caracteres conhecidos por todas as linguagens humanas. Basicamente, isso pode lidar com todo conteúdo em texto que você colocar.

&lt;title&gt;&lt;/title&gt; — isso é o título que aparece no topo de browser quando sua página carrega, é o título dela que aparece na aba do seu navegador.

&lt;nav&gt; - indicar regiões da página que contêm links de navegação pelo site.

&lt;main&gt; -  conteúdo principal da página.

&lt;header&gt; - cabeçalho da página ou de uma região dela.

&lt;footer&gt; - mesma ideia da tag "header" só que neste caso para o rodapé.

&lt;article&gt; - conteúdo que, por si só, já tem um sentido completo, como um post de um blog ou uma notícia.

&lt;section&gt; -  parte/seção de uma página ou texto.

### Indentação, para que serve?

Indentar o código \(com margens diferentes para cada elemento\) é algo para tornar mais visual a hierarquia das informações. Isso porque o HTML têm uma ordem que determina o comportamento dos elementos. Então é colocado cada item em caixinhas dentro de caixinhas.

![](/assets/hmtl.png)

## Elemento pai e filho

Quando começa a programar é bem comum aparecer elemento pai e filho durante explicações, vídeos...mas o que seria? Nada mais é que um tipo de hierarquia no seu código que ajuda na hora de trabalhar no CSS. Com a ajuda da indentação, fica muito mais claro o que é pai e filho dentro de um html.

![](/assets/2018-01-11 %283%29.png)

## CSS

O CSS tem como principal função estilizar seu site, ou seja, deixar ele bonito e personalizado da maneira que você imagina seu site. Ele ajuda também na usabilidade do seu site, e em uma melhor experiência de navegação. A forma de escrever seu CSS é diferente do html, e inserido em um arquivo diferente, geralmente nominado como styles.css.

![](/assets/2018-01-13.png)

![](/assets/codecss.png)

Ele é referenciado em seu HTML através da tag &lt;link&gt; :

```
<link rel="stylesheet" href="style.css">
```

E através de um seletor, é colocado as propriedades que você que aplicar na tag escolhida, como cor de texto, cor de fundo, largura, espaçamento...

## Itens mais utilizados no CSS

* `.classes{  }`

Uma classe é reutilizável: pode se repetir na página e também combinar-se com outras \(podemos pôr mais de uma classe em um elemento\)

* `#ids{  }`

\#id é uma identificação única: só pode ser utilizada uma vez no documento inteiro. Normalmente é utilizada para identificar elementos estruturais da página.

* `.minha-classe p{  }`

* `display: flex;`

* `position: relative;`

* `position: absolute;`

* `@media(max-width: 600px){}`

## Exemplos de propriedades do CSS

* `color: black`

* `background-color: blue`

* `margin: 0 20px 30px 3px`

* `text-align: center`

## Dicas para o CSS

* Utilizem várias classes em uma mesma tag

```
//HTML
<section class="text-center container">
<h1>Meu Título</h1>
</section>

//CSS
.text-center {
  text-align: center;
}
.container{
  margin: 0 15%;
}
```

* Brinquem com border radius

```
//HTML
<section class="text-center container">
<img src="#" class="bordinha">
<h1>Meu Título</h1>
</section>

//CSS
.text-center {
  text-align: center;
}
.container {
  margin: 0 15%;
}
.bordinha {
  border-radius: 50%;
  border: 1px solid black;
}
```

#### O que é  media queries?

Uma expressão colocada no seu arquivo CSS que limita/adapta a apresentação do seu conteúdo de acordo com um formato especifica de dispositivos \(tamanho da tela\), geralmente usado para largura, altura e cor.

```
@media(max-width: 1024px) and (min-width: 700px){
  container{
    display: flex;
    }
    h1 {
      color: red;
    }
  }

  @media (max-width: 699px){
    container{
      display: flex;
      flex-wrap: wrap;
      }
      h1 {
        color: blue;
      }
  }
```

#### Inserindo cor de fundo - CSS

Para alterar a cor de fundo de algum componente do seu site, a propriedade utilizada é _background-color_:

```
h1 {
background-color: blue;
}
```

Mas e se eu quiser inserir um azul mais claro como um azul piscina? Há ferramentas hoje que te ajudam a informar o número hexadecimal \(\#851944\) de cada cor ou a numeração em RGB \(rgb\(133, 25, 68\)\):

[RGB Calculator](https://www.w3schools.com/colors/colors_rgb.asp)

[Color Picker](https://www.google.com.br/search?q=color+picker)

Chrome Developer Tools

#### Mudando o texto - CSS

Para estilizar seu texto há várias propriedades que você pode utilizar dentro do CSS. Algumas são:

```
text-align;
color;
font-weight;
font-family;
letter-spacing;
text-shadow;
text-decoration;
text-indent;
font-style;
font-size;
```

Para colocar o tamanho da fonte ou de qualquer elemento, podemos trabalhar com pixels, rem, e em.

Em pixels é a medida mais antiga que é utilizada e  mais exata que você vai conseguir definir de um elemento.Por exemplo, se você tiver um layout de um site criado em Photoshop você vai conseguir ver a medida em px e aplicar o mesmo em seu site.

Já o em é uma medida tipográfica, e ajuda muito quando você vai criar site para grandes telas ou aplicativos, pois é ajustado o elemento dentro do seu elemento pai, ou seja, imagina uma &lt;div&gt; que tem o tamanho de 40px\(contexto\) e dentro desta div consta um &lt;p&gt; com tamanho da letra de 14px\(target\), o tamanho em em seria 2.85em.

Para saber a medida basta dividir o valor do elemento que você quer mudar que seria o seu target e dividir pelo seu elemento pai que neste caso o valor da div.

E se for para saber a medida da div, o valor de 40px seria dividido por 16px onde daria 2.5em.

E por que 16px? Esta medida é uma medida default onde 1em equivale a 16px.

Existe também o rem que é semelhante ao em porém ele se referencia ao elemento raiz do html, que seria a tag &lt;html&gt;,

e em porcentagem que pode-se referir ao altura, largura ou o elemento pai.

#### Incorporando elementos

* exercício de incluir mapa e um vídeo em seu html

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Meu primeiro site</title>
  </head>
  <body>
    <h1>
      Meu primeiro site!
    </h1>
    <p>
      Eu estou aprendendo a programar.
    </p>
    <p>
      Eu posso escrever qualquer coisa nestes parágrafos.
    </p>
    <p>
      <b>Este é um texto com negrito</b>!
    </p>
    <p>
    <img src="rocketship.gif" alt="foguete"/>
    </p>
    <p>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/sx_C9jJ0AlA" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>
    </p>
    <p>
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d112100.62837159118!2d-51.85816535560437!3d-28.59543745955916!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x951d914036458fdd%3A0x84b2df5f3853d32d!2sPara%C3%AD+-+RS!5e0!3m2!1spt-BR!2sbr!4v1513037488637" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
    </p>
  </body>
</html>
```

A tag &lt;iframe&gt;  são como quadros que podem ao ser adicionados no conteudo de uma página HTML, exibem o conteúdo de uma outra página, como um exemplo, um vídeo que esteja no Youtube.

**width=  **é** **o largura do IFRAME, onde pode ser tanto em pixels quanto porcentagem, por exemplo: 100px.

**height= **é a altura do IFRAME, onde pode ser também tanto em pixels quanto porcentagem, por exemplo 200px.

**frameborder= **Diz a espessura da linha divisória que aparece entre a página e o IFRAME. Sendo o valor deve ser em pixels ou 0.

**scrolling = 'yes', 'no', 'auto' - **Determina se aparecerá barra de rolagem. O auto é quando a barra de rolagem só aparecerá quando o conteúdo da página ultrapassar o tamanho.

#### Criando links para outras páginas no seu html

Neste ponto aprendemos a tag anchor \(Âncora\) que é &lt;a&gt; para implementar um link, como um exemplo de fazer uma parte do seu texto dentro do seu parágrafo virar um link para um outro site.

O atributo href faz parte da tag, tem a função de referenciar algo externa que será requisitado no momento que a pessoa clicar por exemplo. Quando você está em um site que tem um "Inscreva-se" sublinhado, ao clicar será direcionado para a página de cadastro correspondente.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Meu primeiro site</title>
  </head>
  <body>
    <h1>
      Meu primeiro site!
    </h1>
    <p>
      Meu link para me adicionar no <a href="https://www.facebook.com">Perfil do Facebook</a>.
    </p>
    <p style="color:blue;">
      Eu estou aprendendo a programar.
    </p>
    <p style="color:red;">
      Eu posso escrever qualquer coisa nestes parágrafos.
    </p>
    <p style="color:green;">
      Este é um texto com <b>negrito</b>!
    </p>
    <p>
    <img src="rocketship.gif" alt="foguete"/>
    </p>
    <p style="border-style:solid;padding:16px;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/sx_C9jJ0AlA" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>
    </p>
  </body>
</html>
```

### Espaçamento

Para trabalhar o espaçamento entre os elementos, o mais comum é os atributos padding e margin.

![](/assets/paddingemargin.gif)

A margin seria o distanciamento do seu elemento com o seu site \(body\) que pode ser tanto colocada em % ou pixel.

```
p {
margin-top: 20px;
}

#elemento {
margin: 10px;
}
```

Em alguns casos só a medida de um dos lados, ou como no segundo exemplo é colocado apenas 'margin' e um valor que será equivalente para todos os lados. Para colocar em todos os lados, basta inserir desta forma abaixo, seguindo o movimento do relógio.

`#elemento { margin: top right bottom left }`

Se 2 valores forem utilizados o primeiro se aplica às bordas verticais \(superior e inferior\) e o segundo se aplica às bordas horizontais \(esquerda e direita\).

```
margin: 10px 20px;         /*  10px acima e abaixo  */
                           /* 20px esquerda e direita */
```

Quando 3 valores são utilizados o primeiro se aplica à borda superior, o segundo será utilizado tanto para a borda esquerda quanto para a borda direita. O terceiro será aplicado à borda inferior.

```
margin: 10px 3% 20px;      /*  10px acima          */
                           /*  3% esquerda e direita */
                           /*  20px abaixo       */
```

Já o padding é o espaçamento interno deste elemento, em todo elemento existe uma borda que pode ser ou não definida que serve como um direcionamento do espaço que será ocupado em seu site.

Seguindo o mesmo conceito do margin, pode ser colocado em % e pixels e definido o valor de todos os lados, ou de apenas um ou definir a medida de cada um.

### Posicionamento

* `display: inline`: permite posicionar os elementos um do lado do outro. Uma desvantagem é que os elementos não aceitam que sejam modificadas as propriedades`width`e`height`.

* `display: inline-block`: permite os elementos se posicionarem um do lado do outro porém, diferentemente do`display: inline`ele permite que os elementos tenham sua`width`e`height`modificadas.  Uma desvantagem de usar`display: inline-block`é espaçar os elementos entre si. Para fazer isso temos que colocar`margin`.

* `float`: O`float` empurra o elemento para um dos lados`(left | right)`e os elementos que estão em baixo sobem. Pode ser uma alternativa para posicionar 2 elementos como &lt;div&gt; uma ao lado da outra.

* `display: flex`: Ele permite os elementos ficarem um do lado do outro, permite espaçar os elementos de forma mais intuitiva. Além disso ele também permite alinhar os elementos verticalmente de forma fácil. O`display flex`pode ser um pouco mais complicado de usar tendo em vista que existem diversas propriedades que vem junto da especificação`flexible box.`

A flex box traz uma otimização quanto ao trabalho de posicionar e espaçar elementos entre si, com propriedades já pré-definidas é possível organizar elementos dentro de um elemento pai. O básico para começar a mexer com flexbox é saber que tem 2 formas de elemento: o container, que é como uma caixinha, e os elementos, que ficam dentro dela. Container é um elemento com classe “container”, que não precisa ser div, pode ser por exemplo ul, section etc. Já os itens estão dentro do container e podem ser qualquer tipo de elemento, como div, li etc e não precisam obrigatoriamente de uma classe específica.

Abaixo listo as ordem possíveis a serem adicionadas ao elemento de classe container. Caso não será declarada, a propriedade será igual ao elemento sinalizado como padrão automaticamente.

**display:**deve ser flex para tudo funcionar certinho.

**flex-direction:**define a ordem dos itens.

* row \(**padrão**\): exibe os itens em linha, em ordem normal
* row-reverse: os itens ficam em linha, mas em ordem reversa
* column: exibe os itens em uma coluna, ou seja, um abaixo do outro
* column-reverse: coluna, mas com ordem reversa

**flex-wrap:**define a quebra de linha

* nowrap \(**padrão**\): não permite quebra de linha
* wrap: permite quebra da linha
* wrap-reverse: quebra a linha, mas na ordem reversa

**justify-content:**alinha os itens horizontalmente

* flex-start \(**padrão**\): alinha os itens no início do container
* flex-end: alinha os itens no fim do container
* center: alinha os itens no centro do container
* space-between: alinha os itens no centro do container, deixando o primeiro e o último grudados nos cantos
* space-around: alinha os itens no centro do container, deixando o mesmo espaço de cada lado para cada um. Nos itens no centro, há um espaçamento 2x maior que os nos cantos.

##### Alguns sites para entender e ver outros exemplos de flexbox e grids layouts:

[https://imasters.com.br/css/adeus-flexbox-bem-vindo-css-grid-layout](https://imasters.com.br/css/adeus-flexbox-bem-vindo-css-grid-layout)

[https://www.chiefofdesign.com.br/flexbox-css3/](https://www.chiefofdesign.com.br/flexbox-css3/)

##### Responsividade

Ter a preocupação em que seu site seja responsivo já é quase uma obrigação de todo desenvolvedor. O conceito Mobile First é um item que tem q estar no escopo de todo projeto.

Há algumas técnicas que podemos utilizar em nosso código para ajudar nesta compatibilidade, e que o seu site tenha um layout responsivo.

Para que suas imagens e/ou vídeos se adaptem de acordo com o layout, uma solução é usar o max-width, que força a imagem em a se redimensionar de acordo com o tamanho do container que ela se encontra.

```
img {
max-width: 100%
}
```

Há também as **medias queries **são expressões de CSS utilizadas para mudar o layout em diferentes dispositivos sem mudar o conteúdo. E como usar em seu CSS? Em resumo os atributos seriam como um tutorial do que você precisa que aconteça em um determinado dispositivo.

## Resolução de tela

Se você quiser desenvolver um CSS tendo um dispositivo específico em mente basta você saber a resolução de uma tela \(altura e largura em pixels\). Hoje no mercado há muitos modelos de celulares por exemplo, mas as medidas são aproximadas de largura e com isso podemos considerar as seguintes larguras:

* **￼320 pixels** – Smartphones no modo retrato.
* **480 pixels** – Smartphones no modo paisagem.
* **600 pixels** – Tablets pequenos. Ex: Amazon Kindle \(600×800\)
* **￼768 pixels **– Tablets maiores em modo retrato. Ex: iPad \(768×1024\)
* **1024 pixels** – Tablets maiores em modo paisagem, monitores antigos.
* **￼1200 pixels** – Monitores

É como se você perguntasse para o browser: “ O seu dispositivo é uma tela e a largura máxima é 320 pixels?”. Se a resposta for sim o navegador aplica o que consta no seu arquivo css.

#### Exemplo do código:

```
/* Smartphone em modo retrato */
@media only screen and (max-width : 320px) {
      /*inserir propriedades CSS */
}
```

```
./* regra aplicada em todo código */
body { background: blue; }

/* aplica somente a partir de 320px */
@media screen and (min-width: 320px) {
   body { font-size: 80%; }
}

/* aplica somente a partir de 480px em landscape */
@media screen and (min-width: 480px) and (orientation: landscape) {
   nav { float: left; }
}
```

## CSS Animation

Animation é uma propriedade de CSS que serve para animar outras propriedades CSS, um exemplo simples é alterar a cor de fundo de verde, para laranja, para rosa e, depois para verde de novo.

@keyframes é uma regra colocada para inserir exatamente para definir qual a transição que o seletor receberá. Por exemplo, se colocar como 0%, e se for no final 100%. Nada impede de ser colocado também nos intervalos, só inserir a porcentagem.

```
.fundo {
  width: 100%;
  height: 100%;
  animation: transition 5s infinite;
}
@keyframes transition {
  0% {
    background-color: #705523;
  }
  100% {
    background-color: #f2e8d5;
  }
}

```

## Hora de colocar em prática seus conhecimentos

Exercício 1

Monte a sua página. Pode ser um currículo, por exemplo uma página com seus hobbies ou coisas preferidas utilizando HTML e CSS.

Exercício 2

Crie uma página que seria um ecommerce. A ideia é ter uma vitrine com produtos e que clicando em algum produto iria para outra página com mais informações sobre este produto. E qual o produto? Você escolhe! Pode ser flores, games, bijouterias...a ideia é estruturar um site com imagens, valores, textos \(pode ser só de marcação\).

Exercício 3

Momento de colocar a responsividade no seu site. Pode ser o site que você já criou o um novo projeto e use media queries. Por exemplo, em telas de celular aparecerá a &lt;nav&gt; de outra cor, ou uma div abaixo da outra...neste momento a ideia é tornar seu site responsivo.

