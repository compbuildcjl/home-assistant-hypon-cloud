ARG BUILD_FROM=ubuntu:22.04
FROM $BUILD_FROM

RUN apk add --no-cache mosquitto-clients

# Copy data for add-on
COPY run.sh /
COPY scripts/ /scripts/

RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
