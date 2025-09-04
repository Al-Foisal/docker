All Docker command

docker run node=>to get pre-build images

docker ps -a => all container process of conainer by docker

docker run -it node => expose an interactive session inside the container to our host machine and this will make interactive terminal where we run node command

docker ps => display all the active container only

docker build . => build custom image based on Docker file

docker run -p <local-port>:<dockerfile-port> <imageid> => this will run the container and run our server

docker run -p <local-port>:<dockerfile-port> --rm <imageid> => this will run the container and run our server and automatically delete container when the container will stop

docker run -p <local-port>:<dockerfile-port> --name <custom-container-name> <imageid> => this will run the container and run our server with custom container name

docker run -p <local-port>:<dockerfile-port> -d <imageid> => this will run the container and run our server in detached mode

docker run -it <imageid> => this will run the container and able terminal for interactive input even if not attached after that container will stop automatically (-it is the short form of -i and -t)

docker attach <container-name> => attached with running container

docker logs <container-name> => display all the logs under a container

docker logs -f <container-name> => continously display all the logs under a container in attached mode

docker start <container-name> => start the respective container in detached mode by default

docker start -a <container-name> => start the respective container in attached mode

docker start -a -i <container-name> => start the respective container in attached mode and able terminal for interactive input

docker stop <container-name> => stop the respective container

docker rm <container-name> => remove container by placing container name use " "(space) to delete multiple container and seperate them by space

docker rmi <imageid> => remove image by placing imageid use " "(space) to delete multiple image and seperate them by space

docker images => get all the images

docker image inspect <imageid> => get respective image details

docker cp <local-folder>/. <container-name>:/<container-folder> => copy all the file from local machile to to a container

docker cp <container-name>:/<container-folder-path> <local-folder>

docker build -t <image-name>:<image-path> . => custom image name

docker tag <image-name>:<tag-name> <reponame>:<tagname> => rename docker image

docker push <repo-name> => push docker image to DockerHub (you must have to login before push)

docker image prune -a => delete all the images