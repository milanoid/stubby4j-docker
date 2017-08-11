# stubby4j-docker
Dockerized [stubby4j](https://github.com/azagniotov/stubby4j) `Hello World`.


1. pull Docker image from Docker Hub

`docker pull milanoid/stubby4j-docker`

2. start Docker image

`docker start -p 8882:8882 stubby4j-docker`

3. hit the stub API with curl

`curl -X POST http://localhost:8882/hello-world`
```$xml
<?xml version="1.0"?>
<hello-world>
    <greeting>Hello, World!</greeting>
</hello-world>
```

`curl http://localhost:8882/hello-world`
```$json
{"hello world"}
```


