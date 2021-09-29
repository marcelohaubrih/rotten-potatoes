# Desafio 02 Rotten Potatoes

### Criar a imagem, atualizar a imagem de acordo com seu usuário e ewxecutar os comandos abaixo

- Criando a imagem

    ``$ docker build -t marcelohaubrih/rotten-potatoes:v1 src/.``

- Enviando a imagem para o dockerhub

    ``$ docker push marcelohaubrih/rotten-potatoes:v1``

### Iniciar serviços na seguinte ordem
- Banco de Dados MONGODB (Dentro da pasta kind/mongodb)

    ``$ kubectl apply -f .\deployment.yaml``

    ``$ kubectl apply -f .\service.yaml``

- Aplicação WEB (Dentro da pasta kind/web)

    ``$ kubectl apply -f .\deployment.yaml``