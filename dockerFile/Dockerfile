#creates a layer from the alpine Docker image.
FROM alpine
WORKDIR /root/hello-docker
COPY HelloDocker.java /root/hello-docker

#We require jdk to run java progam so we need to install jdk
RUN apk add openjdk8
ENV JAVA_HOME /usr/lib/jvm/java-1.8-openjdk
ENV PATH $PATH:$JAVA_HOME/bin

#Compile our HelloDocker program
RUN javac HelloDocker.java

ENTRYPOINT java HelloDocker
