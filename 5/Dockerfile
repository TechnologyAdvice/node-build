FROM mhart/alpine-node:5

RUN apk update

# npm install deps
RUN apk add git openssh-client

# native build deps
RUN apk add make gcc

# scripting tools
RUN apk add bash

CMD ["/bin/bash"]
