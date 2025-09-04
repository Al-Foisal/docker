# All Docker command

- `docker run IMAGE`: to get pre-build images

- `docker ps -a`: all container process of conainer by docker

- `docker run -it IMAGE`: expose an interactive session inside the container to our host machine and this will make interactive terminal where we run node command

- `docker ps`: display all the active container only

- `docker build .`: build custom image based on Docker file

- `docker run -p LOCAL_PORT:DOCKER_FILE_PORT IMAGEID`: this will run the container and run our server
> - `-p` for publish the image
> - `--rm` for automatically delete container when the container will stop
> - `--name IMAGE` for custom container name
> - `-d` for run our server in detached mode

- `docker attach CONTAINER`: open running container in attached mode

- `docker logs CONTAINER`: display all the logs under a container

- `docker logs -f CONTAINER`: continously display all the logs under a container in attached mode

- `docker start CONTAINER`: start the respective container in detached mode by default

- `docker start -a CONTAINER`: start the respective container in attached mode

- `docker start -a -i CONTAINER`: start the respective container in attached mode and able terminal for interactive input

- `docker stop CONTAINER`: stop the respective container

- `docker rm CONTAINER`: remove container by placing container name use " "(space) to delete multiple container and seperate them by space

- `docker rmi IMAGE`: remove image by placing imageid use " "(space) to delete multiple image and seperate them by space

- `docker images`: get all the images

- `docker image inspect IMAGE`: get respective image details

- `docker cp LOCAL_PATH/. CONTAINER:/CONTAINER_PATH`: copy all the file from local machile to to a container

- `docker cp CONTAINER:/CONTAINER_PATH LOCAL_PATH`: copy from docker container to local machine

- `docker build -t IMAGE_NAME:IMAGE_TAG .`: custom image name

- `docker tag IMAGE_NAME:IMAGE_TAG REPO_NAME:TAG_NAME`: rename docker image

- `docker push REPO_NAME`: push docker image to DockerHub (you must have to login before push)

- `docker image prune -a`: delete all the images