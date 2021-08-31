FROM node:alpine

WORKDIR /usr/app

COPY ./package.json ./
RUN yarn
COPY ./ ./

CMD [ "yarn", "start" ]

# docker build -t brunoalencar/simpleweb .  
# docker run -p 5000:3000 brunoalencar/simpleweb
# docker exec -it containerId sh