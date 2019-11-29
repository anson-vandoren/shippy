FROM alpine:latest

RUN mkdir /app
WORKDIR /app

COPY consignment.json /app/consignment.json
COPY consignment-cli /app/consignment-cli

CMD ["./consignment-cli"]
