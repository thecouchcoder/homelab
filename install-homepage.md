# Installation
I followed the [HomePage docker installation guide](https://gethomepage.dev/installation/docker/) to get started.

I had to update the docker compose to deconflict the ports since Hoarder is already running on port 3000.  I mapped the container port 3000 to the host port 3001 instead.

# Configuration
I skimmed [this Techno Tim video](https://www.youtube.com/watch?v=mC3tjysJ01E) to get an idea of what HomePage can do.  However, I mostly used the HomePage documentation.

I setup both Plex and Hoarder services.

I wanted to show the Docker container status on homepage, so I followed [the instructions to setup a Docker socket proxy](https://gethomepage.dev/configs/docker/#using-docker-socket-proxy).  I was not sure how to reference the container names that are started up in compose, so I played around with [the usage instructions](https://github.com/Tecnativa/docker-socket-proxy/blob/master/README.md#usage) for docker socket proxy.  This led me to connecting my DOCKER_HOST to the running container and doing `docker container ps`, which showed the correct container names.  The format is `{service name}-{container name}`.

To connect the Plex widget I exec'd into the Plex docker container and grabbed the server token for my API Key at this location `$PLEX_HOME/Library/Application Support/Plex Media Server/Preferences.xml`