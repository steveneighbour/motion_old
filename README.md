# motion
Repo to work on a simple but robust Motion container

Run via something like this;

  docker run --name=motion \
    -p 7999:7999 \
    -p 8081:8081 \
    -p 8082:8082 \
    -p 8083:8083 \
    -p 8084:8084 \
    -p 8085:8085 \
    -p 8086:8086 \
    -e TZ="Australia/Brisbane" \
    -v /volume1/motion_docker/config:/usr/local/etc/motion \
    -v /volume1/motion_docker/storage:/var/lib/motion \
    --restart=always \
    motion/motion:latest
    
   docker run --name=motion \
    -p 7999:7999 \
    -p 8081:8081 \
    -p 8082:8082 \
    -p 8083:8083 \
    -p 8084:8084 \
    -p 8085:8085 \
    -p 8086:8086 \
    -e TZ="Australia/Brisbane" \
    -v /volume1/motion_docker/config:/usr/local/etc/motion \
    -v /volume1/motion_docker/storage:/var/lib/motion \
    --restart=always \
    c842515f3c75
