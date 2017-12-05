# Node & Express -Diego e Vagnao



Instalando o NodeJS  - https://nodejs.org/en/

A versão mais recente e recomendada para a maioria dos usuarios  é a 8.9.1 LTS. 

 Windows 

Baixar o instalador e executa-lo. 



Instalando via terminal Linux e macOS

Linux

```
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash - 
```

```
sudo apt-get install -y nodejs
```



macOS

Install Homebrew:

https://brew.sh/

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





