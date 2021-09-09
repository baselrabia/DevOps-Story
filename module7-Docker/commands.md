<h1 align="center" > Docker Commands </h1>


1. `docker ps`  # current containers
2. `docker run` # create and start the container
3. `docker create` # create container
4. `dokcer exec` # to run commnads in container for once
5. `docker stop [container ID]` # terminate the container and save it's state by commit it 
6. `docker rm [container ID]` # remove container 
7. `docker inspect [container ID]` # Get more info about running container
___
7.  `docker images` # list the images
8. `docker push` # push your image to docker repo
9. `docker pull` # download an image from docker repo
10. `docker commit` # create an image from container
11. `docker rmi` # remove image
___
12.  `docker volume` # create a docker volume
13. `docker network` # create a docker network
14. `docker build` # build a new image from dockerfile

___
download nginx image from docker repo </br>
`docker pull nginx:1.10.0`

list the images </br>
`docker images`

check the OS pagckages and search for nginx </br>
`sudo dpkg -l | grep nginx`

run first instance of nginx container </br>
`docker run -d nginx:1.10.0`

to check container up and running </br>
`docker ps`

run new instance of different nginx version inside container even the version is not exist </br>
`docker run -d nginx:1.9.3`


check the OS processes that running  and search for nginx </br>
`ps aux | grep nginx`

get more information about specsific container </br>
`docker inspect [container ID]`

Now you can see the `ip address` and can serve it throw Curl command</br>
`curl http://172.17.0.4`

</br>

```bash
`docker stop` preserves the container in the `docker ps -a` list 
(which gives the opportunity to commit it, if you want to save its state in a new image).

It sends `SIGTERM` first, then, after a grace period, `SIGKILL`.

`docker rm` will remove the container from `docker ps -a` list, 
losing its "state" (the layered filesystems written on top of the image filesystem).
It cannot remove a running container (unless called with "-f", in which case it sends SIGKILL directly).

In term of lifecycle, you are supposed to "stop" the container first, then "remove" it.
It gives a chance to the container PID 1 to collect zombie processes.
```
