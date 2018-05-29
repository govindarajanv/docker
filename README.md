# docker

Ref: Linux Academy, Docker official site

Updated the exercises and solutions for basic Docker handson
docker info

# To remove containers
docker rm -f $(docker ps -a -q)

# To remove images
docker rmi -f $(docker images -a -q)

#To remove volumes
docker volume rm $(docker volume ls -q)

# To remove networks
docker network rm $(docker network ls | tail -n+2 | awk '{if($2 !~ /bridge|none|host/){ print $1 }}')
