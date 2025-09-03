# I will start pulling node image and this allows us to build your own image or up another base-image. Here I am building node image that will exists in my own PC or even on the DockerHub under the same name and by this name Docker will recognize the image.
FROM node

 # The working directory where every thing will happend includig our all the command.
 WORKDIR /app

 # Here the first path(.) implies all the folders, sub-folders and files in the root directory except Dockerfile(here Dockerfile is in root directory) will be copied into the image and the second path(/app) implies, inside the image all the files should be stored. Every image and there every container based on the image has it's own internal file system which is totally detouch from the file system from your local machine. It's better to keep inside a sub-folder(make sub-folder name as WORKDIR) insted of root directory in Docker container.
 COPY . /app

 # This will inastall all the node dependency
 RUN npm install

 # As Docker is isolated and it has it's own internal machanism and when a Docker container start we want to expose a certain port to our local system. As our machine will run this container so we can listen the node server from our local machine on port 80.
 EXPOSE 80
 # CMD stands for Command and this run when a container will start based on image. The difference between RUN & CMD is RUN will execute when image will create and CMD will run when container will start based on image.
 CMD [ "node", "server.js" ]