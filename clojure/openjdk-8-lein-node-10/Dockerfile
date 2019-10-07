FROM clojure:openjdk-8-lein

ENV NODE_VERSION=10

RUN apt-get update
RUN apt-get -y install curl
RUN apt-get -y install sudo
RUN apt-get -y install curl gnupg
RUN curl -sL https://deb.nodesource.com/setup_${NODE_VERSION}.x  | bash -

RUN apt-get -y install nodejs

CMD ["sh", "-c", "lein --version && node --version"]
