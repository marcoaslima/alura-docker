# Docker project

## Tecnologies

## How to run

## Some useful commands
sudo usermod -aG docker $USER;

docker run ubuntu

docker ps -a


docker exec -it #id

docker stop #id
docker start #id

docker pause #id
docker unpause #id

docker rm #id

docker run -it bash

#sem ter que esperar no terminal - não trava mais
docker run -d  dockersamples/static-site

#mapeando portas aleatórias
docker run -d -P  dockersamples/static-site
docker port #id
#mapea porta de forma a dizer qual porta
docker run -d -p 8080:80  dockersamples/static-site

docker images
docker inspect #id

docker build -t marcoaslima/alura-docker:1.0 .

To stop all containers from running:
docker stop $(docker container ls -q)

docker tag  marcoaslima/alura-docker:1.0 marckdx/alura-docker:1.0