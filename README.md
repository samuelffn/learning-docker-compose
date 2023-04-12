# learning-docker-compose
Estudos básicos sobre Docker e Docker Compose.

## Brincando com o Docker

### Usando o Nginx pra testar
docker run --name nginx  -d -p 8080:80 nginx
docker ps ou docker ps -a
docker stop <docker_id> ou <name> 
docker start <docker_id> ou <name>

### Fazendo o build do Dockerfile para gerar a imagem com a aplicação Go lang 
docker build -t samuelfranca/aprendendo-docker .
docker images

### Executando nossa imagem
docker run -d -p 8080:8080 samuelfranca/aprendendo-docker:latest
docker ps

### Testando a aplicação GO
Abra o navegado, acesse: http://localhost:8080


## Brincando com o Docker Compose