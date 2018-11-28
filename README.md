# motion
Repo to work on a simple but robust Motion container

Run via something like this;

  docker run --name=motion \
    -p 8081:8081 \
    -p 8082:8082 \
    -e TZ="Australia/Brisbane" \
    -v /hoststorage/motion/conf:/etc/motion/conf \
    -v /hoststorage/motion/storage:/var/lib/motion \
    --restart=always \
    motion/motion:latest
