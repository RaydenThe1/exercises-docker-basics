FROM ubuntu:24.04

RUN apt update -y && apt install -y curl
WORKDIR /usr/src/app
COPY script.sh .
CMD ["./script.sh"]
