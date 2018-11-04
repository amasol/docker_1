#Talking cow

FROM debian

RUN apt-get update && apt-get install -y cowsay fortune lolcat

ENTRYPOINT /usr/games/fortune | /usr/games/cowsay | /usr/games/lolcat

# docker build -t bex04app .

# docker run --rm -t bex04app

#fortune: fortune is a program that displays a pseudorandom message from a database of quotations that first appeared in Version 7 Unix.
#cowsay:cowsay is a program that generates ASCII pictures of a cow with a message.
#lolcat produces rainbow of colors in terminal.
#Flag -t is important in docker command. Without this flag cow will get no color.