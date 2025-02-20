# Mediabox Docker

It's based on running on an Ubuntu server, but could easily be adapted for other opertaing systems with Docker support.

It includes the following Services

- [Plex Media Server](https://www.plex.tv/) - for managing media and serving files to Plex Clients
- [qBittorrent-pia](https://github.com/j4ym0/pia-qbittorrent-docker/tree/master) + [Private Internet Access](https://www.privateinternetaccess.com/pages/buy-vpn/toz) - for downloading torrents... "safely"
- [Sonarr](https://sonarr.tv/) - for TV Series Management
- [Radarr](https://radarr.video/) - for Movie Management
- [Homarr]() - applications dashboard
- [Traefik](hhttps://traefik.io/) - reverse Proxy and SSL Support

## SSL
### Localhost
Generate local SSL certificates using OpenSSL at the root of your project:
```
openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
-keyout localhost.key -out localhost.crt
```
This will generate 2 files localhost.crt and localhost.key