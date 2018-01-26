# Banco de Dados: MongoDB

## Banco de Dados: relacional X não-relacional

Como o nome já sugere, o banco de dados é uma aplicação dá ao usuário a possibilidade de armazenar e receber dados. A diferença entre os bancos de dados relacional e não-relacional são a forma de inserção de dados e à sua organização interna.

* **Banco de dados relacional: **Aqui, os dados são guardados em forma de tabela: dentro das tabelas, os dados são organizados em colunas, e cada coluna contém um tipo de dado. Cada dado é inserido como uma nova linha na tabela.

![](http://www.totalcross.com/blog/wp-content/uploads/2017/10/Exemplo-Banco-de-Dados.png)

**Obs.: **no modelo relacional, a estrutura do banco de dados deve ser projetada com cuidado, pois não é possível inserir novos tipos de dados depois de pronto. Alguns tipos de bancos relacionais: MySQL e SQL Server.

* **Banco de dados não-relacional: **Os modelos não-relacionais surgiram da necessidade de se ter uma melhor performance e alta escalabilidade. Utilizando um banco não-relacional, não há a necessidade de se fazer toda a arquitetura do banco antes de utilizá-lo, pois todas as informações são ocupadas em um documento \(geralmente um JSON\). Alguns exemplos de bancos não-relacionais: MongoDB \(que usaremos em nossos projetos\) e CouchDB.

![](/assets/Capturar.PNG)

**Obs.: **Perceba que é possível que cada documento tenha quantos parâmetros desejar.

## Utilizando o MongoDB

### Estrutura do MongoDB

![](https://image.slidesharecdn.com/mongodbhalloweenparty-141031014902-conversion-gate01/95/mongo-db-halloween-party-8-638.jpg?cb=1414720310)

O MongoDB possui a estrutura declarada na imagem para organização de seus documentos. No servidor, podemos criar vários bancos de dados, e dentro de um banco de dados, podemos criar várias coleções. Por sua vez, podemos ter, também, vários documentos dentro de uma coleção.

#### Como instalar?\(_Windows_\)

Acesse o site : [https://www.mongodb.com/](https://www.mongodb.com/) e faça o download;

Após a instalação, acesse o prompt de comando e digite o seguinte comando: md \data\db

Este comando cria um diretório para salvar/armazenar seus dados.

Após isso, acessar através do caminho abaixo o mongod que é o seu servidor e mongo, que é a área do mongo que você vai manipular seus dados.

![](/assets/mongo.png)

#### Como instalar?\(_Mac_\)

Acesse o site : [https://www.mongodb.com/](https://www.mongodb.com/) e faça o download;

Após a instalação, acesse o terminal e digite o seguintes comandos:

![](/assets/Captura de Tela 2018-01-26 às 14.38.47.png)

Por padrão, MongoDB escreve / armazena dados na pasta  `/data/db`, você precisa criar esta pasta manualmente e atribuir permissão adequada.

![](/assets/Captura de Tela 2018-01-26 às 14.39.48.png)

Crie um `~/.bash_profile `arquivo e atribua `/usr/local/mongodb/bin `a variável de ambiente **$ PATH**, para que você possa acessar facilmente os comandos do Mongo.

![](/assets/Captura de Tela 2018-01-26 às 14.41.43.png)

_\(obs: para sair e outros comando no **vim**\)_

![](/assets/Captura de Tela 2018-01-26 às 14.46.49.png)



Comece MongoDB com `mongod `e faça uma simples conexão com mongo `mongo`.

![](/assets/Captura de Tela 2018-01-26 às 14.44.33.png)

![](/assets/Captura de Tela 2018-01-26 às 14.48.03.png)





### Documentação MongoDB

Estude a documentação do Mongo através desse link: [https://docs.mongodb.com/manual/tutorial/getting-started/](https://docs.mongodb.com/manual/tutorial/getting-started/)

**Obs.: É muito importante saber ler as documentações de bibliotecas, frameworks e APIs. Não existe apostila melhor para aprender sobre um determinado assunto do que a sua própria documentação. Por isso não vamos ensinar aqui os métodos do MongoDB: todos estão bem explicadinhos na documentação!**

