#Minecraft

FROM debian

RUN apt-get update && apt-get upgrade -y && apt-get install -y wget default-jre

WORKDIR minecraft

RUN wget https://launcher.mojang.com/mc/game/1.13/server/d0caafb8438ebd206f99930cfaecfa6c9a13dca0/server.jar

RUN echo 'eula=true' > eula.txt

EXPOSE 25565

ENTRYPOINT java -Xmx1024M -Xms1024M -jar server.jar

# docker build -t bex03app .

# docker run --rm -d -p 25565:25565 bex03app