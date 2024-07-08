# Multithreaded Proxy Server

This project is a multithreaded proxy server that can handle HTTP GET requests. It listens for incoming connections on a specified port, forwards the requests to the target server, retrieves the responses, and sends them back to the clients. The server utilizes multithreading to handle multiple client connections simultaneously.

## Features

- Handles HTTP GET requests.
- Multithreaded to support multiple clients concurrently.
- Simple command-line interface to specify the port number.

## Prerequisites

- C++ compiler (e.g., `g++`)
- POSIX-compliant operating system (e.g., Linux, macOS)

## Getting Started

### Compilation

To compile the proxy server (although precompiled file is already included), run the following command:

```sh
make all
```

### Running the Proxy Server
To run the proxy server, use the following command:

```./proxy_server <port-no.>```
Replace <port-no.> with the port number you want the proxy server to listen on. For example, to run the server on port 8080:

```./proxy_server 8080```

### Project Structure
proxy_server.cpp: The main source file containing the implementation of the proxy server.
README.md: This README file.

### Usage
Compile the source code using the provided compilation command.
Run the proxy server on a desired port.
Configure your web browser or HTTP client to use the proxy server by specifying localhost and the port number you chose.
Send HTTP GET requests through the proxy server and observe the responses:

Eg:
Run the server on port 8080:
Configure your HTTP client (e.g., curl) to use the proxy server:

```curl -x localhost:8080 http://example.com```
