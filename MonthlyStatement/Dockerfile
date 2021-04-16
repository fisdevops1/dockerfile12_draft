#Dockerfile to launch Java project on Linux
FROM alpine:3.15
RUN apk add openjdk8
ENV PATH $PATH:/usr/lib/jvm/java-1.8-openjdk/bin
WORKDIR /usr/share/demo
ADD monthlyStatement.java monthlyStatement.java
ENTRYPOINT javac monthlyStatement.java && java monthlyStatement
