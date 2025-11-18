# 17th November

## Docker Volume

Allows to persist the data even if the container is restarted or destroyed.

### tmpFS
Is a temporary file system that is not persisted to storage. It is useful for situations where you want to store temporary files or data that should not be persisted.

### Bind Mount
Allows you to mount a file or directory from the host machine into a container. It is useful for situations where you want to share files or directories between the host machine and the container.

### Named Volume
Named volumes are volumes that are created and managed by Docker. They are useful for situations where you want to share files or directories between multiple containers. Named volumes are persisted to storage and can be used to share data between containers.

### Anonymous Volume
Anonymous volumes are volumes that are created on the fly when a container is started. They are not persisted to storage and are only available to the current container. They are useful for situations where you want to store temporary files or data that should not be persisted.


1  docker run -it ubuntu bash
2  docker ps
3  docker run -it ubuntu bash
4  mkdir test
5  cd test
6  echo "Test" >> text.txt
7  exit
8  docker ps
9  docker ps -a
10  docker start 3f
11  docker ps
12  docker exec -it 3fa0955450e8 bash
13  cd test
14  ls
15  cat text.txt
