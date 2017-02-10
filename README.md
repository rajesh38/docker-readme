# docker-readme
#### Reference: https://docs.docker.com/

### Install docker
You can find the installation guide for your environment [here](https://docs.docker.com/engine/getstarted/step_one/)

### How to verify your installation
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

### List docker images:

```
docker images
```

### List docker containers

```
docker ps -a
```

### Pull docker image

```
docker pull <username>/<image-name>
```
e.g. you can pull [`rajesh38/ubuntu-ngrok`](https://hub.docker.com/r/rajesh38/ubuntu-ngrok/)

### Build docker image from `Dockerfile`

```
docker build -t <image-name> .
```
This will build a docker image using the `Dockerfile` in the current directory

### Push docker image
##### step1: login to your docker account as follows. If you dont have one create one [here](https://hub.docker.com/register/)
```
docker login
```
Use your credentials to login
##### step2: rename your image to the format `<username>/<image-name>` using `docker tag` command
```
docker tag <image-id> <username>/<image-name>
```
You can find the `image-id` by running `docker images`

##### step3: docker push
```
docker push <username>/<image-name>
```

### Some usefule notes

* [Docker RUN vs CMD vs ENTRYPOINT](http://goinbigdata.com/docker-run-vs-cmd-vs-entrypoint/)