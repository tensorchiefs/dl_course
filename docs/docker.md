# How to use the docker container for the couse

## Installation of docker

* The official guide can be found at: https://docs.docker.com/engine/installation/
* In addition we have an instruction for Windows at: https://dl.dropboxusercontent.com/u/9154523/zhaw/how.to.docker-v4.pdf


## Running the container
In the docker command line do:
```
docker run -p 8080:8888 -p 8081:6006 -it oduerr/tf_docker
```
open http://localhost:8080 or http://192.168.99.100:8080 (for windows) in the browser. 

## Running with a linked file system.
```
docker run -p 8700:8888 -p 8701:6006 -v /Users/oli/Documents/workspace/dl_cas/:/notebooks/dl_cas/ -it oduerr/tf_docker
```


## Updating
Please make sure to use the latest container by updating it using 
```
docker pull oduerr/tf_docker
```
