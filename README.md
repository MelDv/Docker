# Docker commands

docker ps -a | Lists all containers
docker images | Lists all images
docker pull <image>	| Pulls image from a docker registry called docker hub
docker rm <container-id> | Removes a container, you can use either container name or id
docker rmi <image-id> | Removes an image, you can use either image name or id
docker stop <container-id> | Stops a container, you can use either container name or id
docker run <image> | Runs an image creating a container, you can use either image name or id
docker run -d <image> | Run in the background
docker exec <container-id> | Executes a command inside the container 
