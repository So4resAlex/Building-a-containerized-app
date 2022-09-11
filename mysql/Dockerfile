FROM mysql:5.7

# Adicionando um database (variável de ambiente)
ENV MYSQL_DATABASE Company

# Adicionando os scripts SQL para serem executados na criação do banco
COPY ./database/ /docker-entrypoint-initdb.d/