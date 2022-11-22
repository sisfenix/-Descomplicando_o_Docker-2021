FROM golang AS buildando
WORKDIR /app
COPY *.go ./
RUN go mod init greeter && go build -o meugo 

FROM alpine
WORKDIR /app
COPY --from=buildando /app/meugo /app

ENTRYPOINT ./meugo
