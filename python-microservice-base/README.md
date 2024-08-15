### Simple python docker base container build

##### documentation:
* https://docs.docker.com/language/python/containerize/

##### instructions:
```bash
docker compose up --build
or
docker compose up --build -d (to run in background)

curl http://0.0.0.0:8000
(to test - should return hello world)

ctrl+c to quit instance
or
docker compose down to quit instance
```

##### publish changes to python base container:
* abstract: docker tag ${TAG} ${DOCKER_USERID}/${DEPLOYMENT_NAME}:${VERSION-TAG}
* abstract: docker push ${DOCKER_USERID}/${DEPLOYMENT_NAME}:${VERSION-TAG}
* actuals below:  
```bash
docker images | grep python (to locate image tag)
docker tag eeb2fd4e4742 johnasexton/python-microservice-base:0.0.1
docker push johnasexton/python-microservice-base:0.0.1
```
