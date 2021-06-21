#base golang image built on Alpine distro
FROM golang:alpine
LABEL maintainer="oluseyeo"
#create the directory app
RUN mkdir /go/src/app
#set newly created directory as working directory
WORKDIR /go/src/app
COPY . .

RUN go mod init
RUN go build -o helloworld
#documentation for the port the application exposes for mapping to host
EXPOSE 6111

CMD ./helloworld