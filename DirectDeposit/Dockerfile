#Dockerfile to launch Java project on Linux
FROM alpine:3.12
RUN apk add openjdk8
ENV PATH $PATH:/usr/lib/jvm/java-1.8-openjdk/bin
WORKDIR /usr/share/demo
ADD directDeposit.java directDeposit.java
ENTRYPOINT javac directDeposit.java && java directDeposit $AMOUNT
