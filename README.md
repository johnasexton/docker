# docker
_(Dockerfile management)_

### Images:
* docker - docker build container for CI
* dskel - template for creating new project directories
* gcloudsdk - google/cloud-sdk for GCP CLI work
* gitlab - private source control (github for public)
* nginx - stable load balancer
* terraform - terraform IaC CLI work

### Published container builds:
* [johnasexton/${image} on DockerHub](https://hub.docker.com/u/johnasexton)

### To use:
```bash
cd ~/workspace/johnasexton/docker/nginx
docker build -t johnasexton/nginx:0.0.1 .
docker push johnasexton/nginx:0.0.1
```
