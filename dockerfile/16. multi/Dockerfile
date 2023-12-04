FROM golang:alpine3.18 as golangbuilder
WORKDIR /app/
COPY main.go /app/
RUN go build -o /app/main /app/main.go

FROM alpine
WORKDIR /app/
COPY --from=golangbuilder /app/main /app
CMD /app/main
