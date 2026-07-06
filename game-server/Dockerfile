FROM rm968211/project-zomboid-server-docker-arm64:latest

USER root

COPY --chown=steam:steam game-server/entrypoint.sh /home/steam/entrypoint.sh
COPY --chown=steam:steam game-server/configure-server.sh /home/steam/configure-server.sh
COPY --chown=steam:steam game-server/mods/ZomboidManager /opt/zm-mod

RUN chmod +x /home/steam/entrypoint.sh /home/steam/configure-server.sh

ENTRYPOINT ["/bin/bash", "/home/steam/entrypoint.sh"]
