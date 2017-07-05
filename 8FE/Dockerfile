FROM node:8

RUN apt-get update

# Yarn
RUN curl -o- -L https://yarnpkg.com/install.sh | bash

# PhantomJS
RUN wget https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.1.1-linux-x86_64.tar.bz2
RUN PHANTOMJS_CDNURL=http://cnpmjs.org/downloads tar xvjf phantomjs-2.1.1-linux-x86_64.tar.bz2 && \
    mv phantomjs-2.1.1-linux-x86_64 /usr/local/share && \
    ln -sf /usr/local/share/phantomjs-2.1.1-linux-x86_64/bin/phantomjs /usr/local/bin

# AWS (requires pip)
RUN apt-get install -y python
RUN apt-get install -y python-pip libpython-dev python-dev
RUN pip install awscli
