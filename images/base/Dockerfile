FROM alpine:3.6


# install homebrew
RUN apt-get install build-essential curl file git
    git clone https://github.com/Homebrew/brew ~/.linuxbrew/Homebrew && \
    mkdir ~/.linuxbrew/bin && \
    ln -s ~/.linuxbrew/Homebrew/bin/brew ~/.linuxbrew/bin && \
    eval $(~/.linuxbrew/bin/brew shellenv)

# install aws-cli
RUN apk -v --update add \
        python \
        py-pip \
        && \
    pip install --upgrade awscli==1.17.9 && \
    apk -v --purge del py-pip && \
    rm /var/cache/apk/*
