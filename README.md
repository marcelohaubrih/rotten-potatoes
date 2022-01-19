# Projeto Clonado do repositório do desafio
> git@github.com:KubeDev/rotten-potatoes.git

## Inserir o projeto em um kluster kubernetes
> Usando o Kind como serviço de cluster kubernetes

# Desafio 02 Rotten Potatoes

### Criar a imagem, atualizar a imagem de acordo com seu usuário e executar os comandos abaixo

- Criando a imagem

    ``$ docker build -t marcelohaubrih/rotten-potatoes:v1 src/.``

- Enviando a imagem para o dockerhub

    ``$ docker push marcelohaubrih/rotten-potatoes:v1``

### Iniciar serviços na seguinte ordem
- Banco de Dados MONGODB

    ``$ kubectl apply -f k8s/mongodb/deployment.yaml``

    ``$ kubectl apply -f k8s/mongodb/service.yaml``

- Aplicação WEB 
  
    ``$ kubectl apply -f k8s/web/deployment.yaml``