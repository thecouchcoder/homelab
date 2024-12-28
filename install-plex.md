# Introduction
We have decided to reduce our dependency on streaming services for a number of reasons including cost, inundation by ads, and loss of ownership.  Recently, we started browsing garage sales and it was such a thrill to look for DVDs.  I purchased quite a few Disney movies and decided to setup a Plex server, so we can be our own streaming service.

# Installation
I'm following this [installation guide]](https://pimylifeup.com/plex-docker/)

I used [environment variables in docker compose](https://docs.docker.com/compose/how-tos/environment-variables/variable-interpolation/) to secure my plex claim token.

You can use `docker compose --env-file=../.env config` with the .env file path to ensure your .env file is being used correctly.

I also changed the permissions of the media folder, so I didn't need root access to upload media.

# Commands
`docker compose --env-file=../.env up -d`

# Troubleshooting
The Plex web UI would not load when I tried to setup homepage.  [Fixing the permissions](https://www.reddit.com/r/unRAID/comments/aj7zom/comment/eeuk804/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button) got it working again