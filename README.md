# docker
_(Dockerfile management)_

### Images:
* docker - docker build container for CI
* gcloudsdk - google/cloud-sdk for GCP CLI work
* gitlab - private source control (github for public)
* hello - template for creating new project directories
* nginx - stable load balancer
* openjdk - Java OPENJDK 11.x
* python - v3.x
* terraform - terraform IaC CLI work

### Published container builds:
* [johnasexton/${image} on DockerHub](https://hub.docker.com/u/johnasexton)

### To use:
```bash
#!/bin/bash 
# abstract
cd ${WORKSPACE}/${REPO}/${IMAGEDIR}
docker build -t ${DOCKERUSER}/${IMAGE}:${TAG} .
docker push ${DOCKERUSER}/${IMAGE}:${TAG}
# literal
cd ~/workspace/johnasexton/docker/nginx
docker build -t johnasexton/nginx:0.0.1 .
docker push johnasexton/nginx:0.0.1
```
