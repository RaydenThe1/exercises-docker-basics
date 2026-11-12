FROM ubuntu:22.04
WORKDIR /app

COPY src ./src
COPY package-lock.json package.json .
COPY public ./public

RUN apt update && apt install -y curl
RUN curl -fsSL https://deb.nodesource.com/setup_16.x | bash
RUN apt install -y nodejs
RUN npm install
RUN npm run build 
RUN npm install -g serve
EXPOSE 5001
CMD ["serve","-s","-l","5001", "build"]
