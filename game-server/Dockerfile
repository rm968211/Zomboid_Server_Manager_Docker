FROM ghcr.io/joyfui/project-zomboid-server-docker-arm64:latest

COPY game-server/entrypoint.sh /home/steam/entrypoint.sh
COPY game-server/configure-server.sh /home/steam/configure-server.sh
COPY game-server/mods/ZomboidManager /opt/zm-mod

RUN chmod +x /home/steam/entrypoint.sh /home/steam/configure-server.sh

ENTRYPOINT ["/bin/bash", "/home/steam/entrypoint.sh"]
