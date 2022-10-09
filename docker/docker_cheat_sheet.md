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

7. running a container in detachhed mode

```bash 
docker run -p <port info> -d <image id>
```

8. running a continaer in attached mode

```bash
docker start -a <container name>

8. attach to container running in detached mode

```
bash
docker attach <conatiner name>
```

9. fetch logs printed by a container (shows all past logs)

```
bash
docker logs <container name>
```

10. fetch logs and attach for future logs

```bash
docker logs -f <contianer name>
```

