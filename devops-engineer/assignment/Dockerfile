FROM golang:alpine as builder
ENV GO111MODULE=on
WORKDIR /app
COPY go.mod .
RUN go mod download
COPY . .
RUN CGO_ENABLED=0 GOOS=linux go build

FROM scratch
COPY --from=builder /app/httpserver /app/
EXPOSE 8080
ENTRYPOINT ["/app/httpserver"]
