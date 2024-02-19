FROM golang:latest

WORKDIR /usr/app

COPY go.mod .
COPY go.sum .

RUN go mod download

COPY . .

RUN go build -o main .

CMD ["/usr/app/main"]
