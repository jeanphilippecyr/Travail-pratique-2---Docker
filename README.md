# Travail-pratique-2---Docker

![](https://github.com/jeanphilippecyr/Travail-pratique-2---Docker/blob/main/images/Screenshot%202023-12-04%20093047.png)

Section 1 - étape 2

docker network create mon_reseau

docker run --name apache -p 80:80 --network mon_reseau -d httpd:alpine

docker volume create mongodb

docker run --name mongodb --network mon_reseau -e MONGO_INITDB_ROOT_USERNAME=adminmongo -e MONGO_INITDB_ROOT_PASSWORD=EncoreUneAutreBD -v mongodb:/data/db -d mongo

docker network ls
docker ps

![](https://github.com/jeanphilippecyr/Travail-pratique-2---Docker/blob/main/images/Screenshot%202023-12-04%20095842.png)

docker logs apache
