# react 
 para instalar o nodejs usamos:
```` sh
sudo apt install nodejs
````
 ou para instalar com nvm 
 ```` sh
 sudo apt install wget
 ````
  
 ```` sh
 wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.34.0/install.sh | bash
 ````
 ```` sh
source ~/.profile
 ````
 
 ````sh
 nvm ls-remote
 ````
 selecione a versao
  ````sh
 nvm install 17.4.0
 ````
 para verificar a versão instalada
  ````sh
 node -v
 ````
 
 para desistalar alguma versao com nvm
  ````sh
nvm deactivate
````
 
  ````sh
 nvm uninstall v17.4.0
 ```` 
 
 para instalar os npm usamos:
```` sh
sudo apt install npm
````
 para instalar o create react app usamos os seguinte comando:
```` sh
sudo npm install -g create-react-app

````

 para criar um app react no linux(de base debian) usamos os seguintes comandos:
```` sh
create-react-app nome-da-pasta-app
````
 e para iniciar usamos os seguinte comando: 
```` sh
npm start
````
# mysql
 para instalar usamos:
 ```` sh
  sudo apt install mysql-server mysql-client
 ```` 
 caso nao esta conseguindo acessar va na loja e ative todas as permições para o workbench 
 
 para acessar o MYSQL use:
 ```` sh
 sudo su
 ````
 
 ```` sh
 mysql -u root -p
 ````
 para mudar a senha use:
 
 ``` sh
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'sua senha DO MYSQL aqui';
 ```
 de um restart no mysql
 ``` sh
 service mysql restart
 ```
# Git ssh key config
### git config
 vamos ver primeiro a versao do git
``` sh
git --version
```
 agora vamos configurar o nome e o email
``` sh
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
```

### ssh config
vamos comecar criando uma ssh no seu sistema
```sh
ssh-keygen -t rsa -b 4096 -C "seuemail@exemplo.com"
```
 deve ter criado a sua chave, vamos verificar
``` sh
cat ~/.ssh/id_rsa.pub
```
