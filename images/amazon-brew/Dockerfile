FROM linuxbrew/brew:latest

# install aws-cli
RUN sudo apt-get update && apt-get install -y \
    python python3-pip && \
    pip3 install --upgrade awscli==1.17.9

# update brew 
RUN brew update && brew doctor
