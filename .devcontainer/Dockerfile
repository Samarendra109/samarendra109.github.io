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