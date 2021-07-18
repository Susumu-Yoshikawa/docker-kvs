FROM golang:1.15.14-alpine3.14 as builder
WORKDIR /src
COPY ./main.go /src
RUN go build -o start_appserver main.go

FROM alpine:3.14
COPY --from=builder /src/start_appserver /bin/start_appserver
CMD [ "/bin/start_appserver" ]