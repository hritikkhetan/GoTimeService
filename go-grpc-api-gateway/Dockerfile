# syntax=docker/dockerfile:1

FROM golang:1.19

WORKDIR /app

COPY . .
RUN go mod download

RUN go build -o /go-grpc-api-gateway

EXPOSE 3000

CMD [ "/go-grpc-api-gateway" ]