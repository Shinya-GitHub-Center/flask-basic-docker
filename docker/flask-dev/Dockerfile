# Since poetry installation is done via pip command,
# it will be installed globally, but this is docker version,
# so please do not concern about this global installation.

FROM python:latest
ARG USERNAME=flask-dev
ARG GROUPNAME=flask-dev
ARG UID=1000
ARG GID=1000
RUN groupadd -g $GID $GROUPNAME && \
    useradd -m -s /bin/bash -u $UID -g $GID $USERNAME
ENV PYTHONUNBUFFERED=1
WORKDIR /home/flask-dev
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y vim less tree jq && \
    pip install poetry
USER flask-dev
RUN poetry config virtualenvs.in-project true
USER root
WORKDIR /home/flask-dev/workdir
