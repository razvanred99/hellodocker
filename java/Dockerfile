# Linux image
FROM alpine
WORKDIR /root/hello-world
COPY Main.java /root/hello-world

# Install JDK
RUN apk add openjdk8
ENV JAVA_HOME /usr/lib/jvm/java-1.8-openjdk
ENV PATH $PATH:$JAVA_HOME/bin

# Compile Main.java
RUN javac Main.java

ENTRYPOINT java Main