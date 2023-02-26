# EquiLoad
EquiLoad is a round robin count based load balancer implemented in Go. It distributes incoming traffic across multiple backend servers, ensuring that no single server gets overwhelmed with requests.

# Architecture
The load balancer server is responsible for receiving incoming requests from clients and distributing them across the backend servers. It does this by maintaining a list of backend servers and their current status. When a request comes in, the load balancer server selects a backend server based on its load-balancing algorithm (such as round-robin, least connections, or IP hash). The load balancer then forwards the request to the selected backend server, and returns the response to the client.

<img src="https://user-images.githubusercontent.com/42131682/221437328-8e0d0b30-ef50-441f-8725-a3aa34003164.png" height="200" width="1000" title="hover text">

## Installation and Setup
To use this load balancer, you'll need to have Go installed on your system. You can download it from the official website: https://golang.org/dl/

Then simply run `go run main.go`
