## step 1:Create the docker file
    create the docker image

 ## step 2:
 sudo docker build -t<image name>:tag<pathofthedockerfile>
 Example:
 sudo docker build -t ubuntu:diot241012.01

 ## Step 3: for check created images
 sudo docker images
 sudo docker image ls

 ## Step 4: run image as cotainer
 sudo docker run -it <imagename>  #it interactive mode 

 sudo docker run -it ubuntu:diot241012.01

 ## step -05:
 check running container
 

 sudo docker ps

 sudo docker containerls

 ## Step-06:
 check all the containers (running/existed/stopped)
 sudo docker ps -a 

 sudo docker container ls -a 

## step -07:
 for installation :
RUN apt  update -y && install net-tools -y 

## step 08 
for ping command
apt install iputils-ping
ping <ipaddress

## step 09
for ssh
apt inatll openssh-client


