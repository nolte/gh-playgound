ARG FROM_IMAGE_NAME=docker.pkg.github.com/nolte/vscode-devcontainers/devops:latest
FROM ${FROM_IMAGE_NAME}

USER root

RUN apk add --update-cache \
  nodejs npm \
  && rm -rf /var/cache/apk/* 

RUN curl https://cli-assets.heroku.com/install.sh | sh

USER ${USERNAME}