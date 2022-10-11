# nst-docker-practices
Docker compose practices 

## Docker commands review
```console

docker pull <image_name>:<tag>

docker build -t node-app:v2 .

docker run -it --rm postgres:13.4-alpine bash

docker exec -it <container_id_or_name> bash

docker run -dp 3000:3000 node-app

docker stop <container_id>

docker run -v /home/vagrant/src/docker/node-app/etc:/etc/todos -dp 3000:3000 node-app

docker run -v /home/vagrant/src/docker/node-app/src:/app/src -v /home/vagrant/src/docker/node-app/etc:/etc/todos -dp 3000:3000 node-app

docker login

docker tag <container_id> luisbl/node-app:v2

docker push luisbl/node-app:v2

docker compose up -d

docker logs <container_name>

```