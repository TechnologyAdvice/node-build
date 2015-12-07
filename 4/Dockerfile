FROM mhart/alpine-node:4.2.3

RUN apk update

# npm install deps
RUN apk add git openssh-client

# native build deps
RUN apk add make gcc

# scripting tools
RUN apk add bash

# update NPM (Not stable yet)
# RUN npm install -g npm@3.0-latest

CMD ["/bin/bash"]
