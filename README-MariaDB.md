# README-MariaDB
MariaDB, an open-source relational database is being used during CDX development
of the CDX monitoring strategy. This README outlines how to stand up a Docker 
container where MariaDB (database) and Adminer (Web Admin) can be used for local 
development.

Dependencies:
- Docker
- Web Browser (optional) for ad hoc database administration

On Windows there are two options for using Docker:
- Install Docker Desktop for Windows, (which also installs Hyper-V).
- Install Docker into a hypervisor of your choice, (eg, VirtualBox, Multipass, etc.).


## Run MariaDB as a Docker container

Run via Docker Compose
```
cd ${CDX_PROJECTS}/cdx-env-tools/docker
docker-compose up -d mariadb adminer
```

This will execute the MariaDB server and a web admin tool in a docker container for 
your local development and testing.

No other configuration is necessary.

##### Testing the server

##### Stopping the server

Stop and remove the container
```
docker-compose rm -fsv mariadb adminer
```

##### TODOs:
##### Notes:


