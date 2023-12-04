FROM golang:alpine3.18
ENV APP_PORT=8991

RUN mkdir app
COPY main.go app

EXPOSE ${APP_PORT}/tcp

CMD go run app/main.go
