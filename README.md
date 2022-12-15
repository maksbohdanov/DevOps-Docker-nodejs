# DevOps-Docker-nodejs
DockerHub [repository](https://hub.docker.com/repository/docker/maksss/node-web-app)  
Build an image:
```shell
docker build . -t maksss/node-web-app
```

Run the image with restrictions on usage memory and CPU(512Mb and 2 CPUs):
```shell
docker run -m 512m --cpus=2 maksss/node-web-app
```

Tag image build with tag `imagefirstpush`:
```shell
docker tag maksss/node-web-app maksss/node-web-app:imagefirstpush
```

Push the image to my personal docker repository:

```shell
docker push maksss/node-web-app:imagefirstpush
```