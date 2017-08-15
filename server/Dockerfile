FROM alpine:latest

RUN apk --no-cache add nodejs nodejs-npm && \
    npm install -g json-server

EXPOSE 3000

CMD ["json-server", "/data/db.json", "--routes", "/data/routes.json"]