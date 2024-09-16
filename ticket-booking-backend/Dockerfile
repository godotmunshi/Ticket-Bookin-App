FROM golang:1.22.2-alpine3.19

WORKDIR /src/app

COPY . .


RUN go install github.com/air-verse/air@latest

RUN go mod tidy

CMD go build -o ./tmp/main ./cmd/api/main.go
