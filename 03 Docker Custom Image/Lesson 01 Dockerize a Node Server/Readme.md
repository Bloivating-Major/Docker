```dockerfile
#BASE IMAGE
FROM ubuntu

RUN apt-get update 
RUN apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_18.x -o /tmp/nodesource_setup.sh
RUN bash /tmp/nodesource_setup.sh
RUN apt install -y nodejs

#Copy the source code to docker image
COPY index.js /home/app/index.js
COPY package.json /home/app/package.json
COPY package-lock.json /home/app/package-lock.json

WORKDIR /home/app

RUN npm install
```

We will optimize this image