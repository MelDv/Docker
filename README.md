# Docker commands

| Command  | Meaning |
|-------|--------|
| `docker ps -a` | Lists all containers |
| `docker images` | Lists all images |
| `docker pull <image>`	| Pulls image from a docker registry called docker hub |
| `docker rm <container-id>` | Removes a container, you can use either container name or id |
| `docker rmi <image-id>` | Removes an image, you can use either image name or id |
| `docker stop <container-id>` | Stops a container, you can use either container name or id |
| `docker run <image>` | Runs an image creating a container, you can use either image name or id |
| `docker run -d <image>` | Run in the background |
| `docker exec <container-id>` | Executes a command inside the container  |
| `docker tag <image>:<tag> <newimage>:<newtag>` | Create a tag for saving different versions of the same image locally, or rename image |
| `docker logs -f <image>` | Gives (follow -> f) output logs |
| `pause, unpause, attach, --sig-proxy=false/true` | Log commands |
| `docker rm --force <image>` or `docker kill <image>` and `docker rm <image>` | Kill image
