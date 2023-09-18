# Docker-Ubuntu

## Docker pull
$ `docker pull ubuntu:20.04`

## Run with connected bash with closing and remove after exit
$ `docker run -it --rm --name ubuntu ubuntu:20.04 /bin/bash`

## Run with connected bash with no need remove
$ `docker run -it --name ubuntu ubuntu:20.04 /bin/bash`
$ `docker exec -it ubuntu /bin/bash`

## Run in detached mode
$ `docker run -id --name ubuntu ubuntu:20.04`
$ `docker exec -it ubuntu /bin/bash`

## Saving the docker container state (result --> new image with all changes)
$ `docker commit -p container_id new_container_name`

## Run in detached mode with mounted directories
$ `docker run -v /dir-on-host:/dir-in-container -id --name ubuntu ubuntu:20.04`<br>
$ `docker exec -it ubuntu /bin/bash`

