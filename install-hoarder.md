# Install
I followed [the instructions from their documentation](https://docs.hoarder.app/Installation/docker)

I had to edit the downloaded compose file to point to my shared .env file, since it's not in the same directory as the compose file.

I am also considering at this point if I should have a single compose file for the homelab or if it makes sense to keep everything seperate.  I've decided to keep to seperate for now, since then tinkering with one service can't affect another.

In order for hoarder to be more useful, I'd like to setup a static IP Address for my homelab.