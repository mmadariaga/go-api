# Go REST API - Learning Project

This project is a personal learning exercise to build a simple REST API using Go. The goal is to practice building APIs with the following tools and libraries:

- **[go-chi/chi](https://github.com/go-chi/chi/v5)**: A lightweight, idiomatic HTTP router for Go.
- **[rs/zerolog](https://github.com/rs/zerolog)**: A high-performance, structured logging library.
- **[stretchr/testify](https://github.com/stretchr/testify)**: A testing toolkit for Go with a variety of helpers for assertions and mocking.


## Install & Run
```bash
git clone https://github.com/mmadariaga/go-api.git
cd go-api
# install dependencies
go mod tidy 
# Run tests
go test ./...
# Run the server
go run cmd/api/main.go 
```

## Features

Currently, the API only has two routes:
- `GET /ping`: Returns a simple "pong" response.
- `GET /races`: Returns application_races.Response json object with a summary of all the races of the year 2024 in f1. This endpoint requires Basic Auth

Example:
```bash
$ curl http://localhost:8080/ping
pong
```

## TODO

 - [ ] Use goroutines to fetch data from third party APIs faster
 - [ ] Enhance test coverage.

## Licence
This project is licensed under the MIT License - see the LICENSE file for details.