# See here for image contents:
FROM mcr.microsoft.com/devcontainers/python:3.7
WORKDIR /workspaces/app

ARG WORKSPACE_FOLDER="/workspaces/app"
VOLUME $WORKSPACE_FOLDER/.venv

ENV DAGSTER_HOME="/workspaces/app"

EXPOSE 3000

RUN apt-get update && apt-get install -y \
    build-essential \
    software-properties-common \
    && rm -rf /var/lib/apt/lists/*
