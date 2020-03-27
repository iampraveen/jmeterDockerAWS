# jmeterDockerAWS
This is a initial distributed load testing setup using docker on AWS. 

## Overview and scope

The scope of this document is to offer a step-by-step tutorial on how to create a distributed load testing infrastructure using AWS EC2, Docker and JMeter.

## Prerequisites
Some basic knowledge of each of the systems mentioned above (EC2, Docker & JMeter) is required to be able to transition from one step to another.
Also, an active AWS account is required to be able to follow through with all the steps.

There are 2 layers we need to build:
A base layer, which creates the elementary setup required to run a JMeter instance.
Another layer on top of the base which can either be a JMeter master or slave instance depending on our needs



#### Create an image and tag:

```docker build -t username/reponame:imageTag /path/to/dockerfile```

#### To create a new container:

```sudo docker run -dit --name containername repository:tag or imageId /bin/bash```


#### To start/stop a container:

```docker start/stop containerId```


#### To access a running container:

```docker exec -it containerId or containerName /bin/bash```

#### Reference: 
1. https://qautomation.blog/2020/01/14/load-testing-with-jmeter-docker-and-aws-ec2/
2. https://dzone.com/articles/how-to-build-a-distributed-load-testing-infrastruc
3. https://github.com/kubernauts/jmeter-kubernetes/tree/master/openshift


