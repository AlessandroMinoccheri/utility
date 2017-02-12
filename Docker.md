#Docker:

## Install inside port 8080
```
docker run -d --name yournamewhatyouwant -p 8080:80 tutum/hello-world
```

## View All Container active
```
docker ps
```

## View Container active
```
docker ps -a
```

## View Images
```
docker images
```

## Delete Container
```
docker rm {containerID}
```

## Delete Image
```
docker rmi {imageID}
```

## View project
localhost:8080

## Create more container example
```
docker run -d --name yournamewhatyouwant -p 8080:80 tutum/hello-world
docker run -d --name yournamewhatyouwant -p 8080:80 tutum/hello-world
docker run -d --name yournamewhatyouwant -p 8080:80 tutum/hello-world

```

## Start a docker
```
docker stop yournamewhatyouwant
```

## Stop a docker
```
docker stop yournamewhatyouwant
```
