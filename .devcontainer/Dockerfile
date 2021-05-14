ARG VARIANT="14"
FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:${VARIANT}

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
     && apt-get -y install --no-install-recommends cmake libicu-dev libidn11-dev python3-docutils ruby ruby-dev \
     && rm -rf /var/lib/apt/lists/* \
     && gem install commonmarker github-linguist github-markup licensee
