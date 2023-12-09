# Golang gRPC Project

This repository contains a Golang project with gRPC implementation. Follow the steps below to set up and run the project.

## Clone Repository

```bash
git clone https://github.com/eduardylopes/fc-grpc
cd fc-grpc
```

## Install Dependencies

```bash
go mod tidy
```

## Sqlite3 Installation

Install the sqlite3 by following the instructions [here](https://www.sqlite.org/quickstart.html).

## Database

In the root folder executes the following commands to create categories table.

```bash
sqlite3 db.sqlite "create table categories (id string, name string, description string);"
```

## Protocol Buffer Installation

Install Protocol Buffers compiler (protoc) by following the instructions [here](https://grpc.io/docs/protoc-installation/).

## Run the project

```bash
go run cmd/grpc_server/main.go
```

## Testing using a gRPC client

To test this app use the gRPC client Evans by following the instructions [here](https://github.com/ktr0731/evans).

## Generate Services and Update Contracts

Follow the instructions [here](https://grpc.io/docs/languages/go/quickstart) to generate new services or modify existing contracts.
