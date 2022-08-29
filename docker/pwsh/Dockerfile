FROM mcr.microsoft.com/powershell:lts-alpine-3.14

RUN apk update && apk add bash

ARG CUSTOM_USER=pwsh
ARG CUSTOM_ID=1000
ARG HOMEDIR=/home/$CUSTOM_USER

RUN addgroup -g $CUSTOM_ID $CUSTOM_USER
RUN adduser -u $CUSTOM_ID $CUSTOM_USER -G $CUSTOM_USER -H -D -h $HOMEDIR
USER $CUSTOM_USER
WORKDIR $HOMEDIR

ENV PATH=$PATH:/opt/microsoft/powershell/7-lts

## Make service always running
CMD exec /bin/bash -c "trap : TERM INT; sleep infinity & wait"
