Jenkins installation in docker:

```sh

docker run --name myjenkins -d \
-p 8082:8080 \
-p 50000:50000 \
-v /var/run/docker.sock:/var/run/docker.sock \
-v jenkins_home:/var/jenkins_home \
jenkins/jenkins:lts


```

```sh
docker run -p 8082:8080 -p 50000:50000 -d -v \
jenkins_home:/var/jenkins_home \
jenkins/jenkins:lts
```
jenkins plugin installation setup:

```https://stackoverflow.com/questions/65242609/jenkins-on-ubuntu-unknownhostexception-when-installing-plugins``` 