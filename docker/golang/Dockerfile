FROM golang:1.18-alpine

COPY backend/go.mod /app/go/go.mod
COPY backend/go.sum /app/go/go.sum
WORKDIR /app/go
# Air インストール
# RUN curl -fLo /go/bin/air https://git.io/linux_air \
#   && chmod +x /go/bin/air
RUN ls
RUN go mod download

COPY . /app/go

CMD go run main.go