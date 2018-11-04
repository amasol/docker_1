FROM debian

ARG DEBIAN_FRONTEND=noninteractive
MAINTAINER amasol <amasol@student.unit.ua>

ENV TS3SERVER_LICENSE=accept

WORKDIR /home/teamspeak

EXPOSE 9987/udp 10011 30033

RUN apt-get update && \
	apt-get upgrade -y && \
	apt-get install -y wget bzip2 && \
	wget http://dl.4players.de/ts/releases/3.0.13.4/teamspeak3-server_linux_amd64-3.0.13.4.tar.bz2 && \
	tar -xvf teamspeak3-server_linux_amd64-3.0.13.4.tar.bz2

WORKDIR teamspeak3-server_linux_amd64

ENTRYPOINT sh ts3server_minimal_runscript.sh

# docker build -t ex01app .

# docker run --rm -p 9987:9987/udp -p 10011:10011 -p 30033:30033 ex01app
