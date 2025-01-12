# WebSocket Server

This is a simple WebSocket server implemented in Go using the `gorilla/websocket` package.

## Features

- Upgrade HTTP connections to WebSocket connections
- Handle WebSocket connections
- Echo received messages back to the client after a delay

## Prerequisites

- Go 1.23 or later (https://golang.org/dl/)

## Setup

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/websocket_server.git
    cd websocket_server
    ```

2. Initialize the Go module (if not already done):
    ```sh
    go mod init websocket_server
    ```

3. Get the required dependencies:
    ```sh
    go get github.com/gorilla/websocket
    ```

### Running the Server

1. Run the server:
    ```sh
    go run main.go
    ```

2. The server will start and listen on port `8080`. You should see the message:
    ```
    Websocket server started
    ```

## Usage

- Connect to the WebSocket server at `ws://localhost:8080/ws`.
- The server will echo back any messages it receives after a 3-second delay.