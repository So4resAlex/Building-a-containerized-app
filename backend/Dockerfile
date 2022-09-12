# Derivando da imagem oficial do Python 3.9
FROM python:alpine3.16 

# Definir o workdir
WORKDIR /code

# Mover o arquivo de dependência do projeto para o workdir
COPY ./requirements.txt /code/requirements.txt

# Instalar dependências do projeto
RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt && pip install uvicorn 

# Copiar a pasta do projeto no workdir
COPY ./app /code/app

# Comando para subir o app
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]