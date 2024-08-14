# GOlang-Load-Balancer

Go Round Robin Load Balancer

This is a simple Round Robin Load Balancer implemented in Go. It distributes incoming HTTP requests across a set of backend servers in a round-robin fashion.

Features

Round Robin Algorithm: Distributes requests evenly across all backend servers.

Reverse Proxy: Proxies incoming HTTP requests to backend servers.

Health Check (Basic): Checks if a server is alive before forwarding requests (current implementation always returns true).


Code Structure

LoadBalancer: The core of the load balancer, managing the list of backend servers and distributing requests.

simpleServer: Represents a backend server, including its address and proxy configuration.

getNextAvailableServer(): Implements the round-robin selection algorithm.
