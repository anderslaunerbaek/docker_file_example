# docker_uni

## Create docker image
Be in folder of the ```Dockerfille```:
```
$ ls
#> app.py  Dockerfile  README.md  requirements.txt
```

```
$ docker build -t docker_test .
```

where docker_test is the name tag of the image...

### Spin up the docker image
```
$ docker run -d -p 8012:80 docker_test
```
