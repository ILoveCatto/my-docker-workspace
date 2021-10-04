FROM debian:stable-slim

RUN apt update
RUN apt install curl wget -y
RUN wget https://raw.githubusercontent.com/ILoveCatto/my-docker-workspace/main/Dockerfiles/Test-CI-Egg/entrypoint.sh

USER container
ENV  USER=container HOME=/home/container

WORKDIR /home/container

CMD ["/bin/bash", "/entrypoint.sh"]
