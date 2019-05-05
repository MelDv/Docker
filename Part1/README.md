# Part1
Docker course, part 1 exercises.

:whale: :whale2: :whale: :whale2: :whale: :whale2: :whale: :whale2: :whale: :whale2: 

## Exercise 1.1

docker ps -a  
CONTAINER ID        IMAGE               COMMAND                  CREATED            STATUS              PORTS                          NAMES  
5325d2a16513        telegraf            "/entrypoint.sh tele…"   7 minutes ago       Up 7 minutes        8092/udp, 8125/udp, 8094/tcp   focused_meninsky


## Exercise 1.2
docker images  
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE

docker ps -a  
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

## Exercise 1.3
Command: "basics"  
Message: "This is the secret message"

## Exercise 1.4
docker run --name clockwork devopsdockeruh/exec_bash_exercise  
docker exec -it clockwork bash  
root@0e146d89faf6:/usr/app#  tail -f ./logs.txt   

tai suoraan  
docker exec -it clockwork tail -f ./logs.txt   
Secret message is:  
"Docker is easy"  
Thu, 02 May 2019 18:54:28 GMT  
Thu, 02 May 2019 18:54:31 GMT  
Thu, 02 May 2019 18:54:34 GMT  
Thu, 02 May 2019 18:54:37 GMT  
Secret message is:  
"Docker is easy"  
.  
.  
.  

## Exercise 1.5
docker run -d --name ubu ubuntu:latest sh -c 'while true; do date; sleep 1; done'  
docker exec ubu apt-get update  
docker exec ubu apt-get install -y curl  
docker exec -it ubu bash  
root@6608d65e07ad:/# sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 100; curl http://$website;'  
Input website:  
helsinki.fi  
Searching..  
`<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">` 
`<html><head>`  
`<title>301 Moved Permanently</title>`  
`</head><body>`  
`<h1>Moved Permanently</h1>`  
`<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>`  
`</body></html>`  
root@6608d65e07ad:/# 

## Exercise 1.6
File Dockerfile is used for this exercise. The file DockerfileLearning was just for studying the material.

docker build -t docker-clock . 
docker run -it docker-clock

