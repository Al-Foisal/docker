All Docker command

docker run node=>to get pre-build images

docker ps -a => all container process of conainer by docker

docker run -it node => expose an interactive session inside the container to our host machine and this will make interactive terminal where we run node command

docker ps => display all the active container only

docker build . => build custom image based on Docker file

docker run -p <local-port>:<dockerfile-port> <imageid> => this will run the container and run our server

docker run -p <local-port>:<dockerfile-port> -d <imageid> => this will run the container and run our server in detached mode

docker run -it <imageid> => this will run the container and able terminal for interactive input even if not attached after that container will stop automatically (-it is the short form of -i and -t)

docker attach <container-name> => attached with running container

docker logs <container-name> => display all the logs under a container

docker logs -f <container-name> => continously display all the logs under a container in attached mode

docker start <container-name> => start the respective container in detached mode by default

docker start -a <container-name> => start the respective container in attached mode

docker start -a -i <container-name> => start the respective container in attached mode and able terminal for interactive input

docker stop <container-name> => stop the respective container