# Projeto Nutri Consultoria

#### Projeto desenvolvido como avaliação para o curso de Análise e Desenvolvimento de Sistemas para faculdade SPTECH.

#### Foi utilizada uma API em NodeJs, fornecida pela instituição.

#### Foram utilizadas as linguagens HTML, CSS e Javascript para o desenvolvimento da aplicação.


sudo docker network create nutri-network

sudo docker build -t nutri-mysql .
sudo docker run -d --rm -p 3306:3306 --name nutri-mysql-container --network nutri-network -e MYSQL_ALLOW_EMPTY_PASSWORD=True nutri-mysql
sudo docker run -d --rm -p 3307:3306 --name nutri-mysql-container --network nutri-network -e MYSQL_ROOT_PASSWORD=password nutri-mysql
sudo docker exec -it nutri-mysql-container /bin/bash

sudo docker build -t nutri-api .
sudo docker run -d --rm -p 3333:3333 --name nutri-api-container --network nutri-network nutri-api 


