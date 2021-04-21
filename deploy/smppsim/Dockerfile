FROM alpine:latest

COPY SMPPSim-2.6.11.zip /tmp

WORKDIR /opt/local/SMPPSim

RUN apk --update add openjdk7-jre unzip && \
    unzip /tmp/SMPPSim-2.6.11.zip -d /opt/local && \
    chmod +x startsmppsim.sh && \
    rm /tmp/SMPPSim-2.6.11.zip

ENTRYPOINT ["/bin/sh", "startsmppsim.sh"]