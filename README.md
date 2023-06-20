# What is Docker?
Docker is a free and open platform that offers an immersive experience to developers working on various aspects of software development. It is a containerization platform that allows developers to package code into various deployable units called containers. Docker Engine is the software that oversees the hosting of the containers. The subset of the Moby Project, Docker, helps developers build, run, and deploy containers on the server and the cloud. The container contains a builder, engine, and orchestrator to deliver a seamless application that runs in any environment.
# Containerization
Containerization is OS-based virtualization that creates multiple virtual units in the userspace, known as Containers. Containers share the same host kernel but are isolated from each other through private namespaces and resource control mechanisms at the OS level. Container-based Virtualization provides a different level of abstraction in terms of virtualization and isolation when compared with hypervisors. Hypervisors use a lot of hardware which results in overhead in terms of virtualizing hardware and virtual device drivers. A full operating system (e.g -Linux, Windows) runs on top of this virtualized hardware in each virtual machine instance. 
# Docker Image
It is an executable package of software that includes everything needed to run an application. This image informs how a container should instantiate, determining which software components will run and how. 
# Docker Container
It is a virtual environment that bundles application code with all the dependencies required to run the application. The application runs quickly and reliably from one computing environment to another.
# Docker Registry
The Registry is a stateless, highly scalable server side application that stores and provides us a way to distribute our docker images.

# Build, Run, Deploy, Publish, Distribute
![image](https://github.com/psangrama/DockerCommands/assets/113549457/a71af3d0-168e-4684-a3c3-8e0a72cabc7d)

# Basic taxonomy in Docker
![image](https://github.com/psangrama/DockerCommands/assets/113549457/e9250595-bc53-415d-a7c7-8c6ed7c92e65)

# Docker Commands
List of usable docker commands for everyday life.

| 	Command	 | 	Usage	 | 
| 	:-----:	 | 	:-----:	 |
| 	docker pull	[ImageName]  | 	Pull the image from docker registry.	| 
| 	docker run -it -d [ImageName]  | 	Command to create a container from an image.	| 
| 	docker images or docker image ls	| 	Lists all images from your system.	| 
| 	docker image ls	| 	Lists all images from your system.	| 
| 	docker ps	| 	Lists out	all the running containers in your system. |
| 	docker ps	-a | 	Lists out	all the running and exited containers of your system . |
| 	docker stop [ContainerID]	| 	Stops the container  |
| 	docker rm [ContainerID] | 	Deletes the container. |
| 	docker rmi [ImageID] | 	Deletes the image. |
| 	docker stop $(docker ps -aq)	| 	Command to stop all running containers from your system. |
| 	docker rm $(docker ps -aq)	| 	Command to deletes all containers from your system. |
| 	docker rmi $(docker images -q)	| 	Command to deletes all images from your system. |
| 	docker kill [ContainerID]	| 	Command to kill the container by stopping its execution right away. |
| 	docker exec -it [ContainerID] bash	| 	Command to access the container running |
| 	docker push [Username/Image Name]	| 	Push the image to docker registry |
|   docker build <Path of Docker File> | 	Create an image from the details specified in docker file |
|   docker network ls | 	List the networks in the cluster. (Connect, Disconnect, Prune can be used with this command) |
|   docker history [ImageID] | 	Command to check the history of a docker image. |
|   docker cp src/. container_id:/target | 	Copy from local system to container  |
|   docker cp container_id:/src/. target | 	Copy from container to local system |

