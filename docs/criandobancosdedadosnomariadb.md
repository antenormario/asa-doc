## Criando banco de dados

É importante a criação do banco de dados para guardar as informações necessárias e importantes do nosso site para inciar o mysql digite ('mysql' no terminal):

# Criação do banco de dados

     nome_db = Nome do seu Banco de dados

     create database nome_db
     character set utf8
     collate utf8_general_ci;
     
# Criação de usuário para o banco de dados

        user = Seu usuário
        senha = Sua senha

        create user ‘user’@’localhost’ identified by ‘senha’;
        
# Entregando privilégios para o usuário

       grant all privileges on nome_db.* to ‘user’@’localhost’;
