# Buildando um app conteinerizado

Para este repositório usei o artigo do [Guillaume Falourd](https://www.linkedin.com/in/guillaumefalourd/) disponivel em:

https://www.zup.com.br/blog/docker-na-pratica?utm_source=google-chat&utm_medium=interno&utm_campaign=gc-geral%E2%80%A6  
  
Esse repositório faz parte dos meus estudos em docker, nele utilizei uma imagem do ``python:alpine3.16`` e do ``mysql:5.7`` para criar um simples app que interage com um banco de dados.

## Requisitos 
- [Curl](https://www.cyberciti.biz/faq/how-to-install-curl-command-on-a-ubuntu-linux/)
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Executando 

Para executar siga os passos  abaixo :

1. Instale o ``curl`` caso ainda não tenha  

2. [Instale o docker](https://www.youtube.com/watch?v=4XwzR9vXT5s)
```
curl -fsSL https://get.docker.com | bash 
```

3. Clone o projeto
```
git clone https://github.com/So4resAlex/Building-a-containerized-app.git && cd Building-a-containerized-app
```

4. Uma vez instaladas as dependencias
```
docker-compose up -d 
```

5. Após isso a aplicação estara online e você poderá utilizar as rotas abaixo 
```
http://0.0.0.0/ 
http://0.0.0.0/employees
```
