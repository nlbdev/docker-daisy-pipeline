FROM ubuntu:14.04

MAINTAINER Jostein Austvik Jacobsen

WORKDIR /home/root/

# Install dependencies
RUN sed -i.bak 's/main$/main universe/' /etc/apt/sources.list
RUN apt-get update && apt-get install -y openjdk-7-jre wget unzip
RUN locale-gen en_US en_US.UTF-8

# Install Pipeline 2
RUN wget https://github.com/daisy/pipeline-assembly/releases/download/v1.9/pipeline2-1.9-webui_linux.zip -O pipeline2.zip && unzip pipeline2.zip

#CMD ["/home/root/daisy-pipeline/cli/dp2", "help"]
