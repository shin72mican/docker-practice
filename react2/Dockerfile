FROM ubuntu:24.04

# COPY . /usr/src/app

WORKDIR /usr/src/app

# 18version install
# RUN apt-get update && apt-get -y install nodejs

# curl install
RUN apt-get update && apt-get -y install curl
# node install
RUN curl -fsSL https://deb.nodesource.com/setup_20.x | bash - &&\
apt-get install -y nodejs

# react install
# 初回時、コンテナ内で以下実行
# yes | npx create-react-app react-app

WORKDIR /usr/src/app/react-app
CMD ["npm", "run", "start"]