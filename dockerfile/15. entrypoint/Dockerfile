FROM golang:alpine3.18

RUN mkdir app

COPY main.go app

EXPOSE 8080

ENTRYPOINT [ "go", "run" ]
CMD [ "/app/main.go" ]
