FROM node:6

RUN apt-get update
ENV NODE_PATH /usr/local/lib/node_modules/

# PhantomJS
RUN wget https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.1.1-linux-x86_64.tar.bz2
RUN PHANTOMJS_CDNURL=http://cnpmjs.org/downloads tar xvjf phantomjs-2.1.1-linux-x86_64.tar.bz2 && \
    mv phantomjs-2.1.1-linux-x86_64 /usr/local/share && \
    ln -sf /usr/local/share/phantomjs-2.1.1-linux-x86_64/bin/phantomjs /usr/local/bin

# AWS (requires pip)
RUN apt-get install -y python
RUN apt-get install -y python-pip libpython-dev python-dev
RUN pip install awscli

# Genesis
RUN npm i -g @technologyadvice/genesis-core --quiet
RUN npm i -g typescript@^2.4.0 --quiet

# Hack: Enzyme attempts to require React from within genesis-core, but it is
# installed inside of the current project. Remove these global installs once
# a solution is found.
RUN npm i -g react@^15.6.1 react-dom@^15.6.1 --quiet
