FROM golang:alpine3.18

RUN apk --no-cache add curl
RUN mkdir app

COPY main.go app

EXPOSE 8080

HEALTHCHECK --interval=5s --timeout=30s --start-period=5s CMD curl -f "http://localhost:8080/health"
CMD go run app/main.go
