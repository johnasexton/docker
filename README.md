# docker
_(Dockerfile management)_

### Images:
* dskel - template for creating new project directories
* nginx - stable load balancer
* gitlab - private source control (github for public) 

### To use: 

```bash
cd ~/workspace/johnasexton/docker/nginx
docker build -t johnasexton/nginx:0.0.1 .
docker push johnasexton/nginx:0.0.1
```
