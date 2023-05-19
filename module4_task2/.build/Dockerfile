# hadolint global ignore=DL3004,DL3007,DL3008,DL3009,DL3015,DL4001,DL4006,SC2046
FROM golang:latest
RUN apt-get update && apt-get upgrade -y \
&& apt-get install -y wget make dpkg curl sudo \
&& wget -q -O hugo_binary.deb https://github.com/gohugoio/hugo/releases/download/v0.111.3/hugo_extended_0.111.3_linux-amd64.deb \
&& sudo dpkg -i hugo_binary.deb \
&& rm hugo_binary.deb \
&& curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s -- -b $(go env GOPATH)/bin  \
&& curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash - && sudo apt-get install -y nodejs \
&& sudo npm install -g markdown-link-check \
&& sudo npm install -g markdownlint-cli