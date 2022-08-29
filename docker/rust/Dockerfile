FROM rust:alpine

RUN apk update && apk add bash

ARG CUSTOM_USER=rust
ARG CUSTOM_ID=1000
ARG HOMEDIR=/home/$CUSTOM_USER

RUN addgroup -g $CUSTOM_ID $CUSTOM_USER
#RUN adduser -u 1000 rust -G rust -H -D -h /home/rust
RUN adduser -u $CUSTOM_ID $CUSTOM_USER -G $CUSTOM_USER -H -D -h $HOMEDIR
USER $CUSTOM_USER
WORKDIR $HOMEDIR

## Make service always running
CMD exec /bin/bash -c "trap : TERM INT; sleep infinity & wait"
