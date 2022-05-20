# Andika Rifqi Istanto - 215611102


Section #1 - Networking Basics

Step 1: The Docker Network Command
 

`$ docker network` 

Step 2: List networks
 

`$ docker network ls`
 
Step 3: Inspect a network
 

`$ docker network inspect bridge`
 
Step 4: List network driver plugins
 

`$ docker info`
 
Section #2 - Bridge Networking

Step 1: The Basics
 

`$ docker network ls`

 

`$ apk update`

 

`$ apk add bridge`

 

`$ brctl show`
 
 

`$ ip a`


Step 2: Connect a container
 

`$ docker run -dt ubuntu sleep infinity`

 

`$ docker ps`

 

`$ brctl show`
 

`$ docker network inspect bridge`
 
Step 3: Test network connectivity
 

`$ ping -c5 172.17.0.2`

 

`$ docker ps`

 

`$ docker exec -it yourcontainerid /bin/bash`


`$ apt-get update && apt-get install -y iputils-ping`
 
 

`$ ping -c5 www.github.com`

`$ exit`

 

`$ docker stop (id container)`
 
Step 4: Configure NAT for external connectivity
 

`$ docker run --name web1 -d -p 8080:80 nginx`
 

`$ docker ps`

 

`$ curl 127.0.0.1:8080`



Section #3 - Overlay Networking

Step 1: The Basics
 

`$ docker swarm init --advertise-addr $(hostname -i)`

 

`$ docker swarm join \`
> --token SWMTKN-1-69b2x1u2wtjdmot0oqxjw1r2d27f0lbmhfxhvj83chln1l6es5-37ykdpul0vylenefe2439cqpf \
> 192.168.0.47:2377

 

`$ docker node ls`
 
Step 2: Create an overlay network
 

`$ docker network create -d overlay overnet`

 
 

`$ docker network ls`
 

`$ docker network inspect overnet`
 
Step 3: Create a service
 

`$ docker service create --name myservice \`
`--network overnet \`
`--replicas 2 \`

 

`$ docker service ls`

 

`$ docker service ps myservice`
 
 

`$ docker network ls`
 
Step 4: Test the network
 

`$ docker network inspect overnet`

 

`$ docker ps`
Melihat spek container network 
Cleaning Up

 

`$ docker service rm myservice`

 

`$ docker ps`

 

`$ docker swarm leave --force`

