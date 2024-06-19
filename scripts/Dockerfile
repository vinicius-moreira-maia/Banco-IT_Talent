# imagem base
FROM mysql:latest

# variáveis de ambiente necessárias para o MySQL
ENV MYSQL_ROOT_PASSWORD=senha_root
ENV MYSQL_DATABASE=nome_bd
ENV MYSQL_USER=usuario
ENV MYSQL_PASSWORD=senha

# Expor a porta 3306
EXPOSE 3306

# Copiar o script SQL para o diretório de inicialização do MySQL
COPY dump.sql /docker-entrypoint-initdb.d/

# criando a imagem
# docker build -t desafio_it_talent_junho_01 .

# executando o container
# docker run -d -p 3306:3306 --name desafio_it_talent_junho_01 desafio_it_talent_junho_01

# executando o shell no container
# docker exec -it desafio_it_talent_junho_01 mysql -u root -p
# a senha fornecida deve ser a senha do root
