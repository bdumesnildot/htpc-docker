# HTPC Docker Setup

This Docker setup is designed to run on an Ubuntu server but can be easily adapted for other operating systems with Docker support. It includes a suite of services for managing media, downloading content, and securing your connection.

## Services Included 📋

- **[Traefik](https://traefik.io/)**: Reverse proxy with SSL support for managing and securing your web services.
- **[Plex Media Server](https://www.plex.tv/)**: Manage and serve media files to Plex clients.
- **[Gluetun](https://github.com/qdm12/gluetun)**: VPN client supporting multiple VPN service providers for secure connections.
- **[qBittorrent](https://www.qbittorrent.org/)**: Torrent client for downloading and managing torrent files.
- **[NZBget](https://nzbget.net/)**: Usenet downloader for managing and downloading Usenet content.
- **[Prowlarr](https://prowlarr.com/)**: Indexer management for Usenet and torrents.
- **[Sonarr](https://sonarr.tv/)**: Automated TV series management.
- **[Radarr](https://radarr.video/)**: Automated movie management.

## Quick start 🚀

1. **Install Docker and Docker Compose**: Ensure Docker and Docker Compose are installed on your server.
2. **Clone the Repository**: Clone this repository to your server.
3. **Configure Environment Variables**: Set up your environment variables in a `.env` (see  `.env.example`)
4. **Create the `traefik_proxy` Network**:
   ```bash
   docker network create traefik_proxy
   ```
5. **Launch the Stack**: Use the following command to launch the services:
   ```bash
   docker-compose up -d
   ```

## Disclaimer ❗️

**Responsibility**: By using this setup, you acknowledge and agree that you are solely responsible for:

- Ensuring compliance with all applicable laws and regulations, including copyright laws.
- Configuring and securing your services to prevent unauthorized access.
- Managing and backing up your data.

**No Warranty**: This setup is provided as-is, without any warranty. The maintainers are not responsible for any data loss, security breaches, or legal issues that may arise from its use.

Use this setup responsibly and at your own risk.
