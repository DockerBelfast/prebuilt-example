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

docker image ls
```


Go to [Docker Hub](https://hub.docker.com/_/jenkins/). View the Tags.


```
docker search jenkins
docker pull jenkins

docker container run -d -p "8080:8080" -v "${PWD}/jenkins_home:/var/jenkins_home" --name my-jenkins jenkins

docker logs my-jenkins
```

Go to port 8080:

Use one time key extracted from logs.
