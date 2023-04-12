# learning-docker-compose
Estudos básicos sobre Docker e Docker Compose.

## Brincando com o Docker

#### Usando o Nginx pra testar  
docker run --name nginx  -d -p 8080:80 nginx  
docker ps ou docker ps -a  
docker stop <docker_id> ou <docker_name>   
docker start <docker_id> ou <docker_name>  

#### Fazendo o build do Dockerfile para gerar a imagem com a aplicação Go lang 
docker build -t samuelfranca/aprendendo-docker .  
docker images  

#### Executando nossa imagem
docker run -d -p 8080:8080 samuelfranca/aprendendo-docker:latest  
docker ps  

#### Testando a aplicação GO
Abra o navegador, acesse: http://localhost:8080


## Brincando com o Docker Compose

#### Executando o nosso docker compose que criamos
docker-compose up -d  
docker-compose down  
docker ps  
docker stop <docker_id> ou <docker_name>   
docker start <docker_id> ou <docker_name>  

#### Testando os serviços que subimos com o docker compose
Teste o Nginx: http://localhost:8080  
Teste a aplicação GO: http://localhost:8081  
  
