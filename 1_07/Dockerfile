FROM ubuntu:24.04

RUN apt-get update -y && apt-get install -y curl
WORKDIR /usr/src/app
COPY script.sh .
ENTRYPOINT ["/bin/bash"]
CMD ["./script.sh"]
