## Managing Images and containers

1. list all the running containers

```bash
docker ps
```

2. list all containers including stopped containers

```bash
docker ps -a
```

3. restart a container

```bash
docker start <container name>
```

4. stop a container
```bash
docker stop <container name>
```

5. build an docker image(when workdir in terminal is project folder)
```bash
docker build .
```

6. build a container and run
```bash
docker run <image id>
```

