# RUn a container with a specific name

sudo docker run -it --name <conatiner name> <image name>
example:sudo docker run -it --name ubdiot ubuntu:iot241012.01

# sudo docker ps 

# install ping
apt install inputils-ping

# How to start a container
sudo docker start<cid/cname>

# How to stop a container
sudo docker stop <cid/cname> 

# How to run command inside a running container
sudo docker exec -it  <cid/cname> <command>

EG: sudo docker exec -it bash

# How to create a image from a container (if a container crash it will give you a data )
sudo docker commit <cname/cid> imagename:tag 

sudo docker images | head - 2

# save  a image for offline sharing
sudo docker save -o ubuntunano.tar ubuntu:nano

sudo docker save ubuntu:nano >ubuntunano.tar

# Load a docker image from a file (like ubuntunano.tar)
sudo docker load -i <filename>

Example: 
sudo docker load -i ubuntunano.tar

# How to push docker image to docker hub
docker tag local-image:tagname new-repo:tagname
eg: docker tag ubuntu:nano sehun/ubuntu:nano

# Make sure docker is logged in,is not use
docker.login

sudo docker push bhupendrajmd/ubuntu:nano

docker push new-repo:tagname

