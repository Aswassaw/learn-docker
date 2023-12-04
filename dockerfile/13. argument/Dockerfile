FROM golang:alpine3.18

ARG app=main

RUN mkdir app
COPY main.go app
RUN mv app/main.go app/${app}.go

EXPOSE 8080

# CMD hanya bisa mengakses ENV, tidak bisa mengakses ARG
ENV app=${app}
CMD go run app/${app}.go
