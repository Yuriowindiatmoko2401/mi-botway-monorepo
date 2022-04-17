FROM node:12.22.7-alpine
WORKDIR /usr/src/app
RUN apk update && apk add --virtual bash coreutils
COPY . .
RUN yarn install
# RUN yarn build
EXPOSE 8080
ENTRYPOINT ["/usr/src/app/entrypoint.sh"]