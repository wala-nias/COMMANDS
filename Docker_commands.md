## Docker Commands:
1. pull images from the docker repository
```
docker pull <image name>
```
2.  create a container from an image
```
docker run -it -d <image name>
```
3. list the running (and exited) containers 
```
docker ps (-a)
```
4. Access the running container
```
docker exec -it <container id> bash
```
5. Stop a running container
```
docker stop <container id>
```
6. Stop container execution immediately
```
docker kill <container id>
```
7. List all the locally stored docker images
```
docker images
```
8. Delete a stopped container
```
docker rm <container id>
```
9. Delete an image from local storage
```
docker rmi <image-id>
```
9. build an image from a specified docker file
```
docker build <path to docker file>
```
