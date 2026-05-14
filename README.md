# Automated-Media
My automated Docker setup for my media server.

PLEASE NOTE I WILL MAKE A AUTOMATED INSTALL SCRIPT LATER ON, I AM VERY BUSY WITH SCHOOL.

A quick overview of how I am running this specific setup.
I am using Ubuntu Server 24 LTS, as I deploy this setup in other locations.
Now as for services on this, Portainer is the web gui. (you could use Arcane, but I don't like it.) 
For the containers, they are setup in stacks for easy deployment, the stacks are the following, ARR, Media, Torrent.
It is needed to say, that I use a network drive as I keep my files located on a seperate system. So, if your drive path is different than what is in my config files, you will need to change that in the YAML.

ARR stack.
This contains all ARR apps, sonarr, radarr, prowlarr, bazarr, (eventually Tdarr, but I am still working out several kinks.)

Torrent stack
Qbittorrent as the torrent download, and gluetun as the proxy. (You will need your VPN credentials for linux, I used NordVPN, which has a differnet username and password from your standard login credentials.)

Media stack
This contains Jellyfin and Jellyseerr (Needs to be updated to Seerr due to the merger, I will update it soon!)
Jellyfin is used as your streaming service. Jellyseerr is used to request your media for your server. 

To my friends who are reading this, enjoy lol.
