# Files

server.go - listens on port 9000 for any grpc clients. When clients call say hello it returns a message
client.go - connects to the server on port 9000. It calls the SayHello method

chat/chat.pb.go - autogenerated file that enables gRPC communication. The file was generate using a command:
protoc --go_out=plugins=grpc:chat chat.proto

Go here to install protoc: https://developers.google.com/protocol-buffers/docs/downloads

Tutorial this code is based on:
https://youtu.be/BdzYdN_Zd9Q?list=PLBMqbbVXi-n1Y2RmVFppQI6lfDHblfbEy

More tutorials: https://grpc.io/docs/languages/go/quickstart/

