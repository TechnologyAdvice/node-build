FROM mhart/alpine-node:6

RUN apk upgrade --update

# Python
RUN apk add python
RUN PYTHON=/usr/bin/python
RUN PATH=$PATH:$PYTHON

# Ruby and jekyll stuff
RUN apk add libatomic readline readline-dev libxml2 libxml2-dev alpine-sdk \
    libxslt libxslt-dev zlib-dev zlib yaml yaml-dev libffi-dev build-base \
    ruby-irb ruby-json ruby-rake ruby-bundler ruby-rdoc ruby-dev ruby-io-console jekyll

# scripting tools
RUN apk add bash

CMD ["/bin/bash"]
