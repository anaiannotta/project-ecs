# Projeto Nutri Consultoria

#### Projeto desenvolvido como avaliação para o curso de Análise e Desenvolvimento de Sistemas para faculdade SPTECH.

#### Foi utilizada uma API em NodeJs, fornecida pela instituição.

#### Foram utilizadas as linguagens HTML, CSS e Javascript para o desenvolvimento da aplicação.




sudo docker build -t nutri-mysql .
sudo docker container run -d --rm -p 3307 -e MYSQL_ROOT_PASSWORD=password --name nutri-mysql-container nutri-mysql
sudo docker exec -it nutri-mysql-container /bin/bash


