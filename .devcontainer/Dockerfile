# Base pytorch image with GPU suport
FROM ubuntu:latest

# Basic package update
RUN apt-get update && apt upgrade -y

# The flag is set to avoid unnecesarry questions during installation
# Example: It asks to set timezone during instalation of python.
ARG DEBIAN_FRONTEND=noninteractive

# Install VIM (For Convenience)
RUN apt-get install -y vim

# Install Git
RUN apt-get -y install git

# Install Brew And Hugo
RUN apt-get -y install curl
RUN '' | /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
RUN echo >> /root/.bashrc
RUN echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"' >> /root/.bashrc
RUN eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
#RUN /home/linuxbrew/.linuxbrew/bin/brew install hugo (Install Hugo)

