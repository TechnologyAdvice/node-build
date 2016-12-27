FROM mhart/alpine-node:6.9

RUN apk update

# npm install deps
RUN apk add git openssh-client

# native build deps
RUN apk add make gcc

# scripting tools
RUN apk add bash

# YARN!
RUN npm i yarn -g

CMD ["/bin/bash"]
