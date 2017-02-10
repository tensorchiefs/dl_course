# How to use the docker container for the course

We provide a docker image [oduerr/tf_docker](https://github.com/oduerr/tf_docker) with [Tensorflow](http://www.tensorflow.org) (v0.12.1) , [TFLearn](http://tflearn.org/), [Keras](https://keras.io/), and many other pre-installed python libraries (numpy, pandas). 

## Installation of docker

* The official installation guide can be found at: [https://docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/)
* In addition we have an instruction for [Windows](https://dl.dropboxusercontent.com/u/9154523/zhaw/how.to.docker-v4.pdf) **Currently Not up to date**


## Running the container
In the docker command line execute:

```
docker run -p 8888:8888 -p 6006:6006 -it oduerr/tf_docker
```
open [http://localhost:8888/?token=tensorchiefs](http://localhost:8888/?token=tensorchiefs) or [http://192.168.99.100:/?token=tensorchiefs](http://192.168.99.100:/?token=tensorchiefs)(for windows) in the browser. 

## Running with a linked file system.
If you want to access a directory here (/Users/oli/Documents/workspace/dl_tutorial/) from inside the docker container execute:

```
docker run -p 8888:8888 -p 6006:6006 -v /Users/oli/Documents/workspace/dl_tutorial/:/notebooks/dl_tutorial/ -it oduerr/tf_docker
```


## Updating
Please make sure to use the latest container by updating it using 

```
docker pull oduerr/tf_docker
```

## Other useful hints for docker

### Starting in bash
In case you want to not start the jupyter notebook sever automatically but want a bash shell do:

```
docker run -p 8888:8888 -p 6006:6006 -it oduerr/tf_docker bash
```

### Local vs Inside container
The entry before the colon ':' is on the local machine, the one after it inside the container. Examples:

```
  docker run -p 4242:8888 -it oduerr/tf_docker #4242 is the port on the local machine, 8888 inside the container
  docker run -v /tmp/dl_tutorial/:/notebooks/dl_tutorial/ #/tmp/dl_tutorial is on local machine
```














