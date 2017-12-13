# Node & Express -Diego e Vagnao

#### O que é Node.js?

É uma plataforma que lê e entende o Javascript pelo lado do browser e também do servidor. Isso torna o processo muito mais ágil. Mas como assim?

Imagine que você tem um site e seu usuário vai fazer o login, ele vai inserir o email e a senha, ou seja, acontecerá uma requisição para o banco de dados para validar e liberar o acesso a outra página. Porém, ao invés de aguardar esta resposta do banco, ele já antecipa a próxima requisição e quando ele receber a resposta é enviado o evento sem deixar as demais requisições paradas e sem sobrecarregar o servidor. O processamento de requisições é muito mais alto e rápido. Por exemplo, um site que utiliza é o Walmart. Imagina na black friday que são milhares de acessos e requisições \(compra, cadastro, pagamento...\) se não tiver um processamento rápido, poderiam perder muitas vendas. 

####  Mas ele então é um servidor no servidor? 

Não. É possível criar um servidor http por exemplo, 





Instalando o NodeJS  - [https://nodejs.org/en/](https://nodejs.org/en/)

A versão mais recente e recomendada para a maioria dos usuarios  é a 8.9.1 LTS.

**Windows**

Baixar o instalador e executa-lo.

Instalando via terminal Linux e macOS

**Linux**

```
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
```

```
sudo apt-get install -y nodejs
```

**macOS**

Install Homebrew:

[https://brew.sh/](https://brew.sh/)

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

NodeJs :

```
curl "https://nodejs.org/dist/latest/node-${VERSION:-$(wget -qO- https://nodejs.org/dist/latest/ 
| sed -nE 's|.*>node-(.*)\.pkg</a>.*|\1|p')}.pkg" > "$HOME/Downloads/node-latest.pkg" 
&& sudo installer -store -pkg "$HOME/Downloads/node-latest.pkg" -target "/"
```

```
brew install node
```

Verificando se foi instalado com sucesso e a versão do Node.js

```
node --version
npm --version
```

Aparecendo a versão do Node.js e do Npm, a instalação foi feita com sucesso.

Obs. O Npm é instalado junto com o Node.js

**Instalando o Express**

[https://expressjs.com/en/starter/installing.html](https://expressjs.com/en/starter/installing.html)

\`\`\`  
$ npm install express --save

