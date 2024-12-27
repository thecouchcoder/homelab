# Installing Diet Pi and AdGuard on a Raspberry Pi

I did not have access to an extra monitor and keyboard, so I decided to do a headless install of DietPi by preconfiguring wifi into the config files and using ssh to complete the setup. I followed this tutorial
https://www.youtube.com/watch?v=vlMpn9u0Y4o
It took a long time due to needing to download many packages from the internet, but overall was easy. I then discovered that Adguard is a built in DietPi software and I was able to select it from the list and have it install and configure for me. Then using the [documentation](https://dietpi.com/docs/software/dns_servers/#adguard-home) I was able to connect to it using port `8083` on the configured static IP Address with username `admin` and the global software password.

# Current Status
I've currently spun this down because the Raspberry Pi was causing major latency issues.  I'll pick it back up in the future.