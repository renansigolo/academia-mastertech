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

É onde são armazenados os dados temporários de sua navegação, para agilizar o acesso aos sites visitados anteriormente. Imagina que seja uma caixinha em que, toda vez que você acessa um site, armazena-se nela dados como pesquisa, cliques, e afins, ou no caso de aplicativos, informações como quais são os aplicativos mais acessados e etc... e cada vez que você acessar um site ou um aplicativo, ele visita essa caixinha para que não tenha que pedir ao usuário todas essas informações novamente. Isso ajuda a economizar tempo e tornar a resposta mais rápida.

Porém é comum que alguns dados se misturem ou que essa caixinha fique com muita informação. Por isso, é muito comum que o browser \(_Google Chrome \_ou_ Internet Explorer, \_por exemplo\) peça para que o usuário apague ou limpe o cache, para eliminar estes dados e ficar mais leve. IMPORTANTE: no cache são dados temporários apenas. Dados como senhas salvas, preenchimento automático e etc se mantém.

### Front-end x Back-end

Quem trabalha com _front-end_ é responsável por toda parte visual, ou seja cores, botões, cliques, e toda interface do site. Nesta etapa é super importante dar atenção a experiência do usuário, chamado de UX \(\_User Experience - \_falaremos sobre isso mais pra frente\).

O foco principal é em HTML \(linguagem de marcação\), CSS \(linguagem de estilo\) e JavaScript \(linguagem de script/programação\). São linguagens _client-side_, ou seja são interpretadas no computador do cliente \(usuário\). Isso significa que não há necessidade de se conectar a um servidor para poder programar com elas, pois não é preciso fazer requisições a bancos de dados nem nada do tipo.

Já quem trabalha com _back-end_ fica na parte de trás, nos bastidores de seu site, na parte de implementação, segurança da informação, performance e com banco de dados também.

As principais linguagens de _back-end_ são C\#, Java, PHP, Python, Ruby... conhecidas também como linguagens _server-side_, linguagens de servidor que fornecem a lógica para cada aplicação. Um exemplo simples é a requisição HTTP: quando um usuário cadastra seus dados em um site, suas informações são salvas em um banco de dados. Para recuperar essas informações, o site faz uma requisição ao banco de dados. Todo esse processo de solicitar a página de cadastro, salvar seus dados e recuperá-los faz parte de uma lógica que é efetuada no _back-end_.

### Aplicações Móveis

São os nossos conhecidos aplicativos de celular. São desenvolvidos exatamente para ser utilizado no mobile e há opções de aplicações nativas, web app e conhecidas como híbridas.

Aplicações nativas são aquelas desenvolvidas na linguagem do sistema operacional, como por exemplo para iOS que usa uma  linguagem própria chamada Swift, para Android seria Java e a grande vantagem é se comunicar melhor com os dispositivos do aparelho, como câmera, pedômetro, entre outros. Isso faz com que a aplicação fique mais funcional, com melhor aproveitamento de energia porém necessita de um conhecimento maior de cada linguagem. A escolha da sua aplicação depende muito da sua necessidade e do seu negócio.

Aplicações web app são sites que se adaptam ao mobile. Ou seja, conseguem mudar sua aparência e a disposição dos elementos do site para que seja mais acessível quando este é acessado em um dispositivo móvel. São aplicativos feitos com HTML, CSS, JavaScript e, se necessário, com as linguagens de _back-end_.

Aplicativos híbridos são feitos tanto para sistemas Android, quanto para iOS. Esse tipo de aplicativo tende a ser mais lento e pesado do que um aplicativo nativo, mas sua vantagem é que pode ser utilizado em qualquer tipo de sistema. Uma solução muito utilizada é o _Ionic_, que é um _framework_ para desenvolvimento rápido e fácil de aplicações híbridas. É o que usamos para criar aplicativos na Academia Mastertech.

### Como a web funciona

![](/assets/import.png)

Clientes são os usuários típicos da Web conectados à Internet, por exemplo, seu computador conectado ao seu Wi-Fi, ou seu smartphone conectado à sua rede móvel.

Servidores são computadores que guardam páginas ou aplicativos. Quando um cliente quer acessar uma página, uma cópia dela é baixada do servidor à máquina do cliente para ser mostrada no browser.

Além do cliente e do servidor, temos:

* **TCP/IP \(**_Transmission Control Protocol e Internet Protocol\)_
  são protocolos de comunicação que definem como os dados viajam pela Web. Isso é como os mecanismos de transporte que te permitem ir ao shopping, fazer um pedido e comprar. Você pode andar e comprar o que você quer, mas nesse caso vamos imaginar que você ligue para a loja, pague seu pedido pelo telefone e espere pela entrega.
* **DNS \(**_Domain Name Servers\)_
  são como listas de endereços para sites. Quando você digita um endereço web no seu navegador, este procura o real endereço da página web no servidor DNS antes de poder lhe entregar a página. O navegador precisa encontrar em qual servidor web a página está hospedada, para que ele mande mensagens HTTP para o lugar certo. Isso é como pesquisar o endereço e o telefone da loja para que você possa entrar em contato.
* **HTTP \(**_Hypertext Transfer Protocol\)_
  é um protocolo de aplicação que define uma linguagem para clientes e servidores conversarem entre si. É como a linguagem que você usa para fazer seu pedido e falar com a pessoa que está entregando seu pedido.
* **Arquivos do componente**
  Um website é feito de muitos arquivos diferentes, que são diferentes partes daquilo que você comprou na loja. Esses arquivos são divididos em dois tipos principais:
  * **Arquivos de Código**: Websites são feitos primariamente de HTML, CSS e JavaScript, e outras tecnologias.
  * **Assets**: Esse é o nome coletivo para todas as outras coisas que compõem um website, como imagens, música, vídeo, documentos PDFs.


  Quando você digita um endereço web no seu navegador:

  1. O navegador vai para o servidor DNS e encontra o verdadeiro endereço onde o site se hospeda.
  2. O navegador manda uma mensagem de requerimento HTTP para o servidor pedindo para enviar a cópia do site ao cliente. Essa mensagem, e todos os outros dados enviados entre o cliente e o servidor, é enviada pela conexão de internet usando TCP/IP.
  3. A partir do momento que o servidor aprova o pedido do cliente, o servidor manda ao cliente a mensagem "200 OK", que significa "Claro que você pode ver esse site! Aqui está", e então começa a enviar os arquivos do site para o browser como uma série de pequenos pedaços chamados pacotes de dados.
  4. O navegador monta os pequenos pedaços em um site completo e te mostra.

# GIT e GITHUB

Comandos Unix/Git

Principais comandos utilizados no terminal

* * `ls` - Exibe todas as pastas e arquivos no diretório atual;

  * `pwd` - Exibe o caminho desde o diretório raiz até o diretório atual;

  * `cd <DiretorioDeDestino>` - Entra no diretório de destino;

  * `cd ..` - Volta um diretório;

  * `mkdir <NomeDaNovaPasta>` - Cria uma nova pasta no diretório atual;

  * `mv <NomeArquivoOuPastaExistente> <NovoNome>` - Altera o nome do arquivo ou pasta;

  * `mv <NomeArquivo.EXTENSÃO> <CaminhoASerMovido/>` - Mover um arquivo do diretório atual para o caminho escolhido. Exemplo: _mv passwd.txt ./Documentos/_ - Move o arquivo passwd.txt para o subdiretório Documentos;

  * `rmdir <NomeDaPasta>` - Apaga uma pasta vazia;

  * `touch <NomeDoArquivo>` - Cria um arquivo;

  * `rm <NomeDoArquivo>` - Apaga um arquivo.

PARA QUEM USA O TERMINAL BASH UBUNTU NO WINDOWS:

* * `cd /mnt/c/` - Acessar o disco C: do windows \(onde ficam seus arquivos\).

**Para subir seu projeto no seu github**

* * `git init` - Inicia um novo repositório git na pasta atual;

  * `git status` - Exibe o status dos arquivos no repositório atual;

  * `git add <NomeDoArquivo>` - Prepara os arquivos selecionados para o _commit_;

  * `git add .` - Prepara os arquivos selecionados para o _commit_;

  * `git commit -m “DESCRIÇÃO DAS ALTERAÇÕES”` - Efetua as alterações no repositório;

  * `git log` - Exibe todos os_ commits_ do repositório local;

  * `git remote` - Exibe os repositórios remotos;

  * `git remote add origin <URL>` - Se você não clonou um repositório existente e quer conectar seu repositório a um servidor remoto \(github\), isso o adiciona e você é capaz de enviar suas alterações para o repositório remoto \(github\);

  * `git push origin master` ou `git push <URL> master` - Empurra as alterações \(_commit_\) para o Repositório Remoto \(Ex: para o GitHub\);

  * `git clone <UrlDoRepositório>` - Copia um repositório para a pasta que você está;

  * `git pull origin master` ou `git pull <URL> master` - Baixa as últimas alterações do repositório remoto;

  * `git help` - é uma ajuda que aparece alguns comandos caso você esqueca qual o correto;

  * `git rm <NomeDoArquivo>` - remove o arquivo selecionado;

  * `git rm -r <NomeDoDiretório>` - remove o diretório do seu projeto, ou seja a pasta do seu projeto;

  * Os nomes de arquivos/diretórios ou extensões de arquivos listados no arquivo **.gitignore **não serão adicionados em um repositório.

Comandos Git: saiba mais em [http://rogerdudler.github.io/git-guide/index.pt\_BR.ht](http://rogerdudler.github.io/git-guide/index.pt_BR.html).

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

* O [Sublime Text](https://www.sublimetext.com/) é um software multiplataforma de edição de texto, no entanto utilizado por muitos desenvolvedores para editar código-fonte, escrito em linguagem Python.

* O [Visual Studio Code](https://code.visualstudio.com/) é um editor de código-fonte desenvolvido pela Microsoft para Windows, Linux e macOS. Ele inclui suporte para depuração, controle Git incorporado, realce de sintaxe, complementação inteligente de código, snippets e refatoração de código.

* [Atom](https://atom.io/) é um editor de texto de código aberto disponível para as plataformas Linux, macOS e Microsoft Windows, desenvolvido pelo GitHub sob a licença MIT.

* [Brackets](http://brackets.io/) é um editor de open-source criado pela Adobe Systems que possui como foco principal o desenvolvimento web.

## Editores online {#editores-online}

* [CodePen](https://codepen.io/)
* [Trinket](https://trinket.io/)
* [JSFiddle](https://jsfiddle.net/)
* [Thimble](https://thimble.mozilla.org/pt-BR/)

# 



