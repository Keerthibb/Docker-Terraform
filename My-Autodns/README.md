**This Project agenda is about to create my own docker image and run the docker container with the specific port.**

**To create image from this Dockerfile**
$ docker build -t myimage .

**Command syntax:**
$ docker run -td{detached mode} --name {custom_name} -p{port} {laptop_port}80:8080{image_port} image_name

**Exact Command**
$ docker run -itd --name autodns --hostname=mydns -p 8082:80 myimage

**Running mulitple containers with the different ports**

$ docker run -itd --name dns-1 --hostname=mydns-1 -p 8081:80 myimage

$ docker run -itd --name dns-2 --hostname=mydns-2 -p 8082:80 myimage

$ docker run -itd --name dns-3 --hostname=mydns-3 -p 8083:80 myimage



