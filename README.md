# Practical example of gRPC implementation
 - Material created in the FullCycle gRPC course, exploring different forms of communication between client and server.

### To update the .proto file
 `protoc --proto_path=proto/ proto/*.proto --plugin=$(go env GOPATH)/bin/protoc-gen-go-grpc --go-grpc_out=. --go_out=.`

### To start the server
  - In the project folder, run `go run cmd/server/server.go`

### To start the client
  - After starting the server, in the project folder run `go run cmd/client/client.go`