# docker-compose
docker-compose up -d
docker-compose down -v
docker-compose down -rmi all -v --remove-orphans
docker-compose start
docker-compose stop
docker-compose restart

# docker
docker images
docker ps -a
docker volume ls
docker start container_name
docker stop container_name
docker rm container_name
docker rmi image_name
docker exec -it container_name /bin/bash
docker logs --tail 1000 container_name
docker logs -f conatiner_name
docker run -d -p 8080:8080 -v host_dir:container_dir --name container_name image_name:version

# dockerfile
docker build -t ifjso/myapp:1.0 .
DOCKER_BUILDKIT=1 docker build -t ifjso/myapp:1.0 .
