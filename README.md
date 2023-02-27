# Minecraft Server Manager Bot
Discord bot that lets you run dockerized minecraft servers.
*NOTE: You must host it yourself, for now at least.*

It is using [itzg/docker-minecraft-server](https://github.com/itzg/docker-minecraft-server).

## You can:
- [x] Configure server properties (inside of `/start` command)
- [x] Run multiple Java Edition versions. (I tested from 1.19.3 to 1.7.10)
- [x] Upload/Download world(s) to/from server.
- [x] Fully use server console in a discord text channel.

## You can't (but its planned ~~somewhat~~)
- [ ] Run multiple server(s) at once.
- [ ] Upload plugins
- [ ] Make `/start` templates.

### HTTP Server
You need an HTTP server (python http.server) to download world(s) from server, because discord sucks and can't give enough file size for bigger wordls.

You can set up one by running:
- `python -m http.server <port>`. Default port is 6969. It should be open if you want to access it outside of local network.

## Configurable
You can configure most of the stuff, just change variables in `config.py` file to your desired ones.
There is more info on what's what in the file.
