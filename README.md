# local-jenkins-docker
Creation of a local jenkins environment using docker


# Steps #

## Docker build ##
docker build -t local_jenkins .

## Docker run ## 
docker run \
-p 8080:8080 -p 50000:50000 \
-v jenkins_home:/var/jenkins_home \
-v /var/run/docker.sock:/var/run/docker.sock \
--name local_jenkins local_jenkins



Browse to localhost:8080
Follow the wizard steps
The inital admin password will be in the output of the container starting
