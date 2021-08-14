FROM node:14-buster

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive  \
    && apt-get -y install --no-install-recommends curl ca-certificates \
    && bash -c "$(curl -fsSL "https://raw.githubusercontent.com/microsoft/vscode-dev-containers/main/script-library/common-debian.sh")" \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*

# i install g de forma global 
RUN npm i -g typescript @angular/cli