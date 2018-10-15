# DockerToolbox
https://www.cnblogs.com/linjj/p/5606687.html
https://mirrors.aliyun.com/docker-toolbox/windows/docker-toolbox/

https://github.com/boot2docker/boot2docker/releases

- docker machine, client, compose, virtual box, kitematic

- Quickstart terminal
- docker images

- docker run -itd --name test1 --network bridge --ip 192.168.56.102 hello-world
- docker run docker/whalesay cowsay boo


# Dockerfile:
- cd Desktop
- mkdir testdocker && cd testdocker
- touch Dockerfile &&notepad Dockerfile

FROM docker/whalesay:latest
RUN apt-get -y update && apt-get install -y fortunes
CMD /user/games/forture -a | cowsay

- docker build -t docker-whale .
- docker run docker-whale


# Git bash
"C:\Program Files (x86)\Git\bin\bash.exe"
"C:\Program Files\Git\bin\bash.exe" --login -i "C:\Program Files\Docker Toolbox\start.sh"

- git bash
- docker-machine create default
- docker-machine ssh default
- docker images


# Boot2Docker
https://www.cnblogs.com/bjfuouyang/p/3798198.html
https://github.com/boot2docker/windows-installer/releases

- boot2docker: script, virtual box, msys
- docker client (boot2Docker-vm)

- sudo docker login
- sudo docker run ubuntu:14.04 /bin/echo 'Hello World'

- docker run hello-world

- boot2docker upgrade
