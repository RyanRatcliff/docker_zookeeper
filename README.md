# Docker Zookeeper
A very basic Docker Zookeeper container.

### To build the container
```
docker build -t ryanratcliff/zookeeper .
```

### Alternatively, the container can be pulled from Docker Registry
```
docker pull ryanratcliff/zookeeper
```

# Example usages

### To startup as is
```
docker run -d ryanratcliff/zookeeper
```

### To startup with data directory located on host
```
docker run -d -v /data/zookeeper:/var/zookeeper ryanratcliff/zookeeper
```

### To startup with data directory located on host and all ports exposed to host
```
docker run -d -P ryanratcliff/zookeeper
```

### To startup with data directory located on host and specific port exposed
```
docker run -d p 2181:2181 ryanratcliff/zookeeper
```
