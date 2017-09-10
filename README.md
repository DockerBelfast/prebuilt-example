Docker prebuilt-example 
=========

Getting started
---------------

Go to [Play with Docker](https://www.play-with-docker.com). You need 1 Instances. 

Run these commands in your instance:
```
git clone https://github.com/dockerbelfast/prebuilt-example.git
cd prebuilt-example
ls

mkdir jenkins_home
ls

docker image ls
```


Go to [Docker Hub](https://hub.docker.com/_/jenkins/). View the Tags.


```
docker search jenkins
docker pull jenkins

docker container run -d -p "8080:8080" -v "jenkins_home:/var/jenkins_home" --name my-jenkins jenkins:2.60.2-alpine

docker logs my-jenkins

docker exec -it my-jenkins /bin/bash
cat /var/jenkins_home/secrets/initialAdminPassword
exit
```

Go to port 8080:

Use one time key extracted from logs.

Notes
---------------
Exceeds memory in Play with Docker
