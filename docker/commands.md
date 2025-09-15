**Create a new Container** 

```
docker run -it [Image-Name]
```

**Exit Docker Container After Entering By Iteractive Mode** 

```
Ctrl + D
```

**List all active Container**

```
docker container ls
```

**List all Container** 

```
docker container ls -a
```

**Start a Container** 

```
docker start [Container-Name]
```

**Run a Container With Source Code Home Path As Volumn For Live Update** 

```
sudo docker run -p 8000:8000 -v "$(pwd):/app" -v /app/node_modules --name=[container-name] [image-name]
```

**Stop a Container** 

```
docker stop [Container-Name]
```

**Stop a Container Forcefully** 

```
docker stop -f [Container-Name]
```

**Delete a Container** 

```
docker rm [Container-ID]
```

**Delete All Stoped Container** 

```
docker container prune
```

**Delete All Container** 

```
sudo docker rm -f $(docker ps -aq)
```

**Execute a Command inside a Container**

```
docker exec [Container-Name] [Command]
```

**Attach the Container shell to the Computer shell** 

```
docker exec -it [Container-Name] bash
```

**Show All the local image**

```
docker images
```

**Delete a local image**

```
sudo docker image rm -f [Image-Name]
```

**Build an Image** 

```
sudo docker build -t [Image-Tag] .
```

**Run A new Container with env variable and port mapping**  

```
docker run -it -e PORT=4000 -p 4000:4000 test
```

**Docker Login** 

```
docker login
```

**Push Image**

```
docker push [Repo-Name]:[tagname]
```

**Docker compose run**

```
docker compose up
```

**Docker compose remove** 

```
docker compose down
```
**Docker compose run in background** 

```
docker compose up -d
```


**Docker run  a container with name**

```
docker run -it --name my_container busybox
```


