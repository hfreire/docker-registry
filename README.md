# Docker Registry
Private docker-registry within docker

## Clone git repo and change directory
1. `git clone https://github.com/hfreire/docker-registry.git`
2. `cd docker-registry`

## Create directory to store data
`mkdir -p /var/lib/docker/registry`

## Create a user account
`docker run --entrypoint htpasswd registry:2 -Bbn <username> <password> > htpasswd`

## Use docker compose to start the registry container
`docker-compose up -d`
