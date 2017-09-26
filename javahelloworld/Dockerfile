FROM openjdk:8-jdk
LABEL maintainer="s.fernandes@lectra.com"

ENV FOO bar

COPY src /home/root/javahelloworld/src
WORKDIR /home/root/javahelloworld
RUN mkdir bin
RUN javac -d bin src/HelloWorld.java
ENTRYPOINT ["java", "-cp", "bin", "HelloWorld"]

RUN apt-get update && apt-get install -y vim
