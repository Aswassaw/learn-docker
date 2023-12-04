FROM golang:alpine3.18

RUN mkdir /app

RUN addgroup -S nbrgroup
RUN adduser -S -D -h /app nbruser nbrgroup
RUN chown -R nbruser:nbrgroup /app

USER nbruser

COPY main.go /app
EXPOSE 8080
CMD go run /app/main.go
