# syntax=docker/dockerfile:1

FROM golang:1.19

WORKDIR /app

COPY . .
RUN go mod download

RUN go build -o /go-rabbitmq-consumer

EXPOSE 50052

CMD [ "/go-rabbitmq-consumer" ]