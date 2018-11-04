#NodeJS_npm_yarn

FROM ubuntu

RUN apt-get update && apt-get upgrade -y && apt-get install -y nodejs npm git vim

RUN npm install yarn --global && npm install npm --global

# docker build -t bex01app .

# docker run --rm -ti bex01app

# Fast: Yarn caches every package it has downloaded, so it never needs to download the same package again. It also does almost everything concurrently to maximize resource utilization. This means even faster installs.
# npm is a package manager for the JavaScript programming language. It is the default package manager for the JavaScript runtime environment Node.js.
# npm & yarn are used ad Node.js package managers