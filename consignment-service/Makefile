build:
	protoc -I. --go_out=plugins=micro:$(GOPATH)/src/github.com/anson-vandoren/shippy/consignment-service \
		proto/consignment/consignment.proto
	docker build -t consignment-service .

run:
	docker run -p 50051:50051 \
		-e MICRO_SERVER_ADDRESS=:50051 \
		consignment-service
