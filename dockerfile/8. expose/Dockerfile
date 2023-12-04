FROM golang:alpine3.18

RUN mkdir app
COPY main.go app

EXPOSE 8998/tcp

CMD go run app/main.go
