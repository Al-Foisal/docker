All Docker command

docker run node=>to get pre-build images

docker ps -a => all container process of conainer by docker

docker run -it node => expose an interactive session inside the container to our host machine and this will make interactive terminal where we run node command

docker ps => display all the active container only

docker build . => build custom image based on Docker file

docker run -p <local-port>:<dockerfile-port> <imageid> => this will run the container and run our server

docker stop <container-name> => stop the respective container