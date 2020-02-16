FROM debian:buster
LABEL maintainer="Xueyuan, Jiang <alexxyjiang@gmail.com>"
LABEL version="pyenv"
ENV LANG=C.UTF-8 LC_ALL=C.UTF-8 DEBIAN_FRONTEND=noninteractive
RUN apt-get update --fix-missing \
  && apt-get install -y git build-essential binutils
RUN apt-get update --fix-missing \
  && apt-get install -y python3-dev python3-pip redis-server
COPY start_servers.sh /start_servers.sh
CMD ["sh", "/start_servers.sh"]
