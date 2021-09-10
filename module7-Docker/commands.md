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
12. `docker tag [OPTIONS] IMAGE[:TAG] [REGISTRYHOST/][USERNAME/]NAME[:TAG]` #  tag an image into a repository 
___
13.  `docker volume` # create a docker volume
14. `docker network` # create a docker network
15. `docker build` # build a new image from dockerfile

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

___



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
___

Disply the help `-h` of the command tag it will tell you all the attrbites it ill take </br>
`docker tag -h` tag an image into a repository 

- `docker tag [OPTIONS] IMAGE[:TAG] [REGISTRYHOST/][USERNAME/]NAME[:TAG]` , `-F` to force 
- `docker tag monolith:1.0.0 kelseyhightower/monolith:1.0.0` 

- `docker push kelseyhightower/monolith:1.0.0`push to dockerhub
- `docker login`

___

### # health checks for k8s

-  `cat pods/healthy-monolith.yaml` - Readiness probe preformed - before container start
-  `kubectl describe pods healthy-monolith | grep Readiness` - Readiness checked 
-  `kubectl describe pods healthy-monolith | grep Liveness` - Liveness probe preformed  - after container start
___

### # add label to pod so service can know where to redirect the request

if we had 2 pods 1-monolith 2-secure-monolith 
and both had the `app:monolith` label 

and we created a service had `app:monolith` and `secure:enabled` labels then 
when we curl any pod with it's external ip it will not response 

so we should add  `secure:enabled`  label to the pod we expose to use with our service

- `kubectl label pods secure-monolith "secure:enable"`
___
