# How to use the docker container for the course

We provide a docker image [oduerr/tf_docker:tf1_py3](https://github.com/oduerr/tf_docker) with [Tensorflow](http://www.tensorflow.org) (v1.0.0) , [TFLearn](http://tflearn.org/), [Keras](https://keras.io/), and many other pre-installed python libraries (numpy, pandas). 

## Installation of docker

* The official installation guide can be found at: [https://docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/)
* For hints how to use docker on Windows see [here](https://www.dropbox.com/s/ml979yxv273iml1/how.to.use.docker.on.windows-after.installation.21032017.pdf?dl=1)
* In case that the docker installation does not work we have an addition installation guide for installing Tensorflow directly on [Windows](https://www.dropbox.com/s/ozxzzx9yt3660tl/install-tensorflow-directly-on-Windows.pdf?dl=1).


## Running the container
In the docker command line execute:

```
docker run -p 8888:8888 -p 6006:6006 -it oduerr/tf_docker:tf1_py3
```
open [http://localhost:8888/?token=tensorchiefs](http://localhost:8888/?token=tensorchiefs) or [http://192.168.99.100:8888/tree?token=tensorchiefs](http://192.168.99.100:8888/tree?token=tensorchiefs)(for windows) in the browser. 

## Running with a linked file system.
If you want to access a directory here (/Users/oli/Documents/workspace/dl_tutorial/) from inside the docker container execute:

```
docker run -p 8888:8888 -p 6006:6006 -v /Users/oli/Documents/workspace/dl_tutorial/:/notebooks/local/ -it oduerr/tf_docker:tf1_py3
```


## Updating
Please make sure to use the latest container by updating it using 

```
docker pull oduerr/tf_docker:tf1_py3
```

## Other useful hints for docker

### Starting in bash
In case you want to not start the jupyter notebook sever automatically but want a bash shell do:

```
docker run -p 8888:8888 -p 6006:6006 -it oduerr/tf_docker:tf1_py3 bash
```

### Local vs Inside container
The entry before the colon ':' is on the local machine, the one after it inside the container. Examples:

```
  docker run -p 4242:8888 -it oduerr/tf_docker:tf1_py3 #4242 is the port on the local machine, 8888 inside the container
  docker run -v /tmp/dl_tutorial/:/notebooks/dl_tutorial/ #/tmp/dl_tutorial is on local machine
```














