FROM ubuntu:16.04
WORKDIR /website
COPY frontend-example-docker .
EXPOSE 5000
RUN apt update && apt install -y curl 
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs 
RUN npm install && npm update 
CMD npm start
