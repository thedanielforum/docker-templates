FROM golang:1.8

ENV APP_NAME app
ENV GOBIN /go/bin

RUN mkdir -p /go/src/$APP_NAME
WORKDIR /go/src/$APP_NAME
COPY . /go/src/$APP_NAME

RUN ["go", "install", "main.go"]

ENTRYPOINT ["main"]

# Port to expose for exsternal conenctions
EXPOSE 8080
