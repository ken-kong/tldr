# docker

> Manage Docker containers and images.
> Homepage: <https://docs.docker.com/engine/reference/commandline/cli/>.

- List currently running docker containers:

`docker ps`

- List all docker containers (running and stopped):

`docker ps -a`

- Start a container from an image, with a custom name:

`docker run --name {{container_name}} {{image}}`

- Start or stop an existing container:

`docker {{start|stop}} {{container_name}}`

- Pull an image from a docker registry:

`docker pull {{image}}`

- Open a shell inside of an already running container:

`docker exec -it {{container_name}} {{sh}}`

- Remove a stopped container:

`docker rm {{container_name}}`

- Fetch and follow the logs of a container:

`docker logs -f {{container_name}}`

- Copy a file or directory from the container's file system to local machine

`docker cp {{container_name}}:{{src_path}} {{dest_path}}|-`

- Copy a file or directory from local filesystem to the container.

`docker cp {{src_path}}|- {{container_name}}:{{dest_path}}`
