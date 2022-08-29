FROM haskell:slim-buster

RUN apt-get update -y && apt-get upgrade -y

ARG CUSTOM_USER=haskell
ARG CUSTOM_ID=1000
ARG HOMEDIR=/home/$CUSTOM_USER

RUN groupadd -g $CUSTOM_ID $CUSTOM_USER
RUN useradd --uid $CUSTOM_ID -g $CUSTOM_USER --shell /bin/bash $CUSTOM_USER

USER $CUSTOM_USER
WORKDIR $HOMEDIR

## Make service always running
CMD exec /bin/bash -c "trap : TERM INT; sleep infinity & wait"
