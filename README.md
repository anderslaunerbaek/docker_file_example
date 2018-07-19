# docker_file_example

## Create docker image
Be in folder of the ```Dockerfille```:
```
$ ls
#> app.py  Dockerfile  README.md  requirements.txt
```
### Bulid the docker image from the ```Dockerfile```

```
$ docker build -t docker_test .
```

where docker_test is the name tag of the image...

### Make the docker image public
```
$ docker tag docker_test anderslaunerbaek/docker_test:latest
$ docker push anderslaunerbaek/docker_test:latest

```


### Spin up the docker image
```
$ docker run -d -p 8012:80 anderslaunerbaek/docker_test
```
expose on port 8012
