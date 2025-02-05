**Create a new Container** 

```
docker run -it [Image-Name]
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

**Execute a Command inside a Container**

```
docker exec [Container-Name] [Command-Name]
```

**Attach the Container shell to the Computer shell** 

```
docker exec -it [Container-Name] bash
```

**Show All the local image**

```
docker images
```

**Build an Image** 

```
docker buildx build -t [Image-Name] .
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
