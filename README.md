
Para rodar o projeto

1 Criar a imagem Docker
Abra um terminal na pasta onde está o Dockerfile e execute o seguinte comando para criar a imagem:

docker build -t ambev-frontend-reactjs .

2️ Rodar o contêiner
Agora, execute o seguinte comando para rodar o contêiner a partir da imagem criada:

docker run -d -p 3001:80 --name ambev-container-reactjs ambev-frontend-reactjs

3. Parar o container Excluir o container e imagem
docker stop ambev-container-reactjs
docker rm ambev-container-reactjs
docker rmi ambev-frontend-reactjs

Agora, acesse no navegador:
http://localhost:3001
