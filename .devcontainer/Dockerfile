#FROM adoptopenjdk:11-hotspot

FROM mcr.microsoft.com/java/jdk:13u1-zulu-ubuntu

LABEL maintainer="@spboyer"
LABEL description="Container for developing Azure Functions with Java using VS Code Remote Containers"
LABEL repo="https://github.com/spboyer/java-azurefunctions-remote-container"
LABEL version="1.0.0"

RUN apt-get update

#insall curl, wget, gnupg and net-tools
RUN apt-get install -y curl wget gnupg net-tools

#install git
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y git

#Install Maven
RUN apt-get -y install maven

#Install the Microsoft package repository GPG key, to validate package integrity
RUN curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
RUN mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg

#Run apt update
RUN apt-get update

#Install the Core Tools package
RUN apt-get install -y azure-functions-core-tools
ENTRYPOINT [ "bash" ]