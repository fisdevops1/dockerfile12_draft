#Dockerfile to launch Java project on Linux
FROM alpine:3.15
RUN apk add openjdk8
ENV PATH $PATH:/usr/lib/jvm/java-1.8-openjdk/bin
WORKDIR /usr/share/demo
ADD instantWithdrawal.java instantWithdrawal.java
ENTRYPOINT javac instantWithdrawal.java && java instantWithdrawal $AMOUNT
