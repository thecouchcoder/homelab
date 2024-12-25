# Introduction
We have decided to reduce our dependency on streaming services for a number of reasons including cost, inundation by ads, and loss of ownership.  Recently, we started browsing garage sales and it was such a thrill to look for DVDs.  I purchased quite a few Disney movies and decided to setup a Plex server, so we can be our own streaming service.

# Installation
I'm following this [installation guide]](https://pimylifeup.com/plex-docker/)

I used [environment variables in docker compose](https://docs.docker.com/compose/how-tos/environment-variables/variable-interpolation/) to secure my plex claim token.

You can use `docker compose --env-file=../.env config` with the .env file path to ensure your .env file is being used correctly.

This error can be fixed with the following command
```
Error response from daemon: error gathering device information while adding custom device "/dev/dri": no such file or directory
```
`sudo mkdir -p ~/dev/dri`
# Commands
`docker compose --env-file=../.env up -d`