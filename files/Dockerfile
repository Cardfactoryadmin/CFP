# Dockerfile

# Author       : CardFactory
# Github       : https://github.com/Cardfactoryadmin
# Messenger    : https://m.me/CardFactory
# Email        : CardFactorykrd@gmail.com
# Date         : 25-08-2021
# Main Language: Python

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/Cardfactoryadmin/CFPhisher"

# Working directory
WORKDIR /CFPhisher/
# Add files 
ADD . /CFPhisher

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "CFPhisher.py", "--noupdate"]

## Wanna run it own? Try following commnads:

## "sudo docker build . -t CardFactory/CFPhisher:latest", "sudo docker run --rm -it CardFactory/CFPhisher:latest"

## "sudo docker pull CardFactory/CFPhisher", "sudo docker run --rm -it CardFactory/CFPhisher"
