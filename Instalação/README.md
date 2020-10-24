## Instalação
Atualize seu Sistema Operacional;

#### sudo apt update

#### sudo apt upgrade

Instalando o docker:

curl -fsSL https://get.docker.com | sh

Instalando do docker-compose

#### sudo curl -L "https://github.com/docker/compose/releases/download/1.25.4/docker-compose-Linux-x86_64" -o /usr/local/bin/docker-compose chmod +x /usr/local/bin/docker-compose

Para verificar o status do docker execute o comando abaixo;

#### sudo systemctl status docker

Caso queira verificar a versão do docker que foi instalado, execute o comando;

#### docker –version

Criando diretório para presistencia de dados e baixando o repositório

#### mkdir opt
#### cd /opt 

#### git clone https://github.com/ricardo98365/GLPI.git

#### cd GLPI 

#### mkdir -p ./var/www/html/glpi \
         #### ./var/lib/mysql

#### chown 472:472 ./var/lib/mysql \
              #### ./var/lib/mysql 
              
Executando os containers

#### docker-compose up -d

Para acesar o GLPI acesse http://<seu_ip>

#### host: mysql

#### usuario: glpi_user

#### senha: glpi

GLPI

#### usuario: glpi

#### senha: glpi
