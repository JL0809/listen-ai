FROM golang:1.23-alpine

WORKDIR /app

COPY . .

RUN CGO_ENABLED=0 go build -v -mod=vendor -o main .

EXPOSE 8002
CMD ["./main"]