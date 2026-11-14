FROM golang
WORKDIR /app

COPY . .

RUN go build
RUN go test ./...

EXPOSE 8080
CMD ["./server"]
