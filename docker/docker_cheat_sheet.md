## Building and Running containers

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
```

8. attach to container running in detached mode

```bash
docker attach <conatiner name>
```

9. fetch logs printed by a container (shows all past logs)

```bash
docker logs <container name>
```

10. fetch logs and attach for future logs

```bash
docker logs -f <contianer name>
```

11. Running a container in interactive mode with a termina
```bash 
docker run -i -t <image id>
```

12. Restarting a container in attached mode with interactive mode
```bash
docker start -a -i <contianer name>
```

## Maintaining Images and containers

1. Removing a container
> cannot removing a running container need to be stopped first

```bash
docker rm <container name/ multiple containers>
```

2. Removing images
> need to remove the containers using those images need to be removed first (stopped and running)

```bash
docker rmi <image id>
```

3. Automatically remove container when stopped

```bash
docker run -p <port info> --rm <image id>
```





