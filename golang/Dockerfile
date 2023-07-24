FROM golang:1.20.6-alpine3.18 as step_1
WORKDIR /app
COPY . .
RUN go mod tidy
RUN go build -o api

FROM alpine
WORKDIR /target
COPY --from=step_1 /app/api /target/api
CMD [ "/target/api" ]
