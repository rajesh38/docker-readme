# docker-readme
1. Reference: https://docs.docker.com/

2. How to verify your installation
```
docker run hello-world
```
What happens with the above command:
 
* The Docker Engine CLI client contacted the Docker Engine daemon.

* The Docker Engine daemon pulled the `hello-world` image from the Docker Hub.

* The Docker Engine daemon created a new container from that image which runs the
executable

* The Docker Engine daemon streamed that output to the Docker Engine CLI client, which sent it
to your terminal.

3. List docker images:
```
docker images
```

4. List docker containers
```
docker ps -a
```
