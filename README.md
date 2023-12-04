# Travail-pratique-2---Docker

Section 1 - étape 2

docker network create mon_reseau

docker run --name apache -p 80:80 --network mon_reseau -d httpd:alpine

docker volume create mongodb

docker run --name mongodb --network mon_reseau -e MONGO_INITDB_ROOT_USERNAME=adminmongo -e MONGO_INITDB_ROOT_PASSWORD=EncoreUneAutreBD -v mongodb:/data/db -d mongo

docker network ls
docker ps

docker logs apache
