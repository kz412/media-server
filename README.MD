# media-server

Full fledged containerised public facing media server, with
* Automatic SSL renewal via LetsEncrypt, using [docker-nginx-auto-ssl](https://github.com/Valian/docker-nginx-auto-ssl)
* Google OAuth using [nginx-google-oauth](https://github.com/cloudflare/nginx-google-oauth)
* [NzbGet](https://nzbget.net/) usenet client
* [NzbHydra](https://github.com/theotherp/nzbhydra) NZB meta-search
* [Sonarr](https://sonarr.tv/) for TV
* [Radarr](https://radarr.video/) for Movies
* [Lidarr](https://github.com/lidarr/Lidarr) for Music
* [Transmission](https://transmissionbt.com/) BitTorrent client

To use, fill out `.env` with appropriate values (see [here](https://github.com/cloudflare/nginx-google-oauth) for more info on how to obtain `NGO_CLIENT_ID`, `NGO_CLIENT_SECRET` and `NGO_TOKEN_SECRET` variables). `PUBLIC_DOMAIN` is the public facing URL for your server.

Tested on Ubuntu Server bionic, currently broken on Windows.


