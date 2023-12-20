FROM node:20-alpine

WORKDIR /app

RUN apk update && \
  apk add git && \
  apk add github-cli && \
  apk add openssh && \
  apk add zsh && \
  apk add curl && \
  npm i -g pnpm && \
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

SHELL ["/bin/zsh", "-c"]