FROM golang:1.16-alpine

WORKDIR /usr/src/app

COPY . .

ENV REQUEST_ORIGIN=https://example.com

RUN go build

EXPOSE 8080

CMD ["./server"]