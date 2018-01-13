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

# GIT e GITHUB

Comandos Unix/Git

Principais comandos utilizados no terminal

* * ls- Exibe todas as pastas e arquivos no diretório atual.

  * pwd- Exibe o caminho do diretório atual \(A\)

  * cdDiretorioDeDestino- entra no diretório de destino

  * cd ..- volta um diretório.

  * mkdirNomeDaPasta- cria uma nova pasta no diretório atual

  * mvNomeArquivoOuPastaExistente NovoNome- Altera o nome do arquivo ou pasta.

  * mvNomeArquivo.EXTENSÃOCaminhoASerMovido/ - Mover um arquivo do diretório atual para o caminho escolhido.EX:mv passwd.txt ./Documentos/ - Move o arquivo passwd.txt para o subdiretório Documentos.

  * rmdirNomeDaPasta- apaga uma pasta vazia

  * touchNomeDoArquivo- cria um arquivo

  * rmNomeDoArquivo- apaga um arquivo

TERMINAL BASH UBUNTU NO WINDOWS:

* * cd /mnt/c/- Acessar o disco C: do windows \(seus arquivos\).

  
**Para subir seu projeto no seu github**

* * git init- Inicia um novo repositório git na pasta atual;

  * git status- Exibe o status dos arquivos no repositório atual;

  * git add NOMEARQUIVO- Prepara os arquivos selecionados para o commit;

  * git add \* OU git add . - \( \* ou . seleciona todos os arquivos\) - Prepara os arquivos selecionados para o commit;

  * git commit -m “DESCRIÇÃO DAS ALTERAÇÕES” -Efetua as alterações no repositório;

  * git log- Exibe todos os commits do repositório local;

  * git remote - exibi os repositórios remotos

  * git remote add origin URL- Se você não clonou um repositório existente e quer conectar seu repositório a um servidor remoto\(github\), isso o adiciona e você é capaz de enviar suas alterações para o repositório remoto\(github\).

  * git push origin master ou git push URL master- Empurra as alterações \(Commit\) para o Repositório Remoto \(Ex: para o GitHub\).

  * git clone UrlDoRepositorio -Copia um repositório para a pasta que você está;

  * git pull origin master ou git pull URL master- Baixa as últimas alterações do repositório remoto;

  * git help - é uma ajuda que aparece alguns comandos caso você esqueca qual o correto.

  * git rm NOMEDOARQUIVO - remove o arquivo selecionado

  * git rm -r NOMEDODIRETORIO - remove o diretório do seu projeto, ou seja a pasta do seu projeto.

  * Os nomes de arquivos/diretórios ou extensões de arquivos listados no arquivo **.gitignore **não serão adicionados em um repositório.

Comandos Git -Saiba mais em:[http://rogerdudler.github.io/git-guide/index.pt\_BR.ht](http://rogerdudler.github.io/git-guide/index.pt_BR.html)

### Extra

## Dicas

* [Live de Front-end e aplicações personalizadas de web](https://www.facebook.com/mastertech.tech/videos/1743943105907692/)
* [Guia completo de Git](http://mastertech.rds.land/live-guia-completo-de-git)
* [Seu primeiro site em Bootstrap](https://www.facebook.com/mastertech.tech/videos/1750683085233694/?id=100000316841119)

### Links de referência

* [BootStrap](https://getbootstrap.com/)

* [JQuery](https://jquery.com/)

* [SASS](http://sass-lang.com/)

* [NPM](https://www.npmjs.com/)

### Links para Consulta

* [W3C Schools](https://www.w3schools.com/)

* [Color Picker](https://www.google.com.br/search?q=color+picker)

* [Roadmap com as últimas tendências em desenvolvimento web para 2017](https://github.com/kamranahmedse/developer-roadmap)

### Para estudar...

* [W3C Schools](https://www.w3schools.com/)

* [Code Schools](https://www.codeschool.com/)

* [Code Academy](https://www.codecademy.com/)

* [https://www.udemy.com/](https://www.udemy.com/) \(alguns cursos são pagos\)

Existem inúmeras ferramentas que podem ser utilizadas para criação e edição de arquivos HTML e CSS, abaixo destaco alguns, fique a vontade para utilizar o seu preferido:

## Editores off-line {#editores-off-line}

* O[Sublime Text](https://www.sublimetext.com/) é um software multiplataforma de edição de texto, no entanto utilizado por muitos desenvolvedores para editar código-fonte, escrito em linguagem Python.

* O[Visual Studio Code](https://code.visualstudio.com/) é um editor de código-fonte desenvolvido pela Microsoft para Windows, Linux e macOS. Ele inclui suporte para depuração, controle Git incorporado, realce de sintaxe, complementação inteligente de código, snippets e refatoração de código.

* [Atom](https://atom.io/) é um editor de texto de código aberto disponível para as plataformas Linux, macOS e Microsoft Windows, desenvolvido pelo GitHub sob a licença MIT.

* [Brackets](http://brackets.io/) é um editor de open-source criado pela Adobe Systems que possui como foco principal o desenvolvimento web.

## Editores online {#editores-online}

* [CodePen](https://codepen.io/)
* [Trinket](https://trinket.io/)
* [JSFiddle](https://jsfiddle.net/)
* [Thimble](https://thimble.mozilla.org/pt-BR/)

# 



