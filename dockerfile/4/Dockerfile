FROM golang
WORKDIR /app
COPY *.go ./
RUN go mod init greeter && go build -o meugo 
ENTRYPOINT ./meugo
