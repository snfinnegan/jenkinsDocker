# jenkinsDocker
Jenkins container containing Docker

docker build -t jenkins-docker .  -- to build image from Dockerfile
docker run -p 8080:8080 -p 50000:50000 -v /var/jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock -name jenkin jenkin-docker
