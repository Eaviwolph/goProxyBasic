FROM golang:1.19-alpine3.16

WORKDIR /app

COPY . .

RUN go mod tidy && go mod vendor

RUN go build -o main .

EXPOSE 8888

CMD ["/app/main"]