FROM node:alpine as builder
WORKDIR '/app'
COPY package.json .
RUN yarn
COPY . . 
RUN yarn build

FROM nginx
COPY --from=builder /app/build /usr/share/nginx/html

# docker build .
# docker run -p 8080:80 db26cbb921c4
