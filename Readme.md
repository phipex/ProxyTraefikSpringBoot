# Proxy Traefik

## Proxy de un servicio con traefik

Configuracion basica de un proxy a un servicio que se espera replicar, para el ejercicio se crea un servicio rest con spring-boot que retorna la ip actual del servicio

## Características

- Contiene dashboard en modo inseguro
- Nivel de log en debug

## Comandos basicos
Se compila la imagen del servicio con el siguiente comando

````
./gradlew build jibDockerBuild  
````
 Se corre el docker compose con el siguiente comando:
 ````
docker-compose up -d
````
Para correr varias replicas del mismo servicio:
````
docker-compose up -d --scale webservice=2
````
# Urls
- Dashboard
  http://localhost:8080/dashboard
  
- Whoami
  http://whoami.docker.localhost/
  
- Webservice
  http://webservice.docker.localhost/greeting
