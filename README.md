# GoLClient

### Overview

GoLClient contains the controller for the Game of Life simulation. My partner and I worked on the following files:
* gol/client.go - contains the controller for communication with the server
* gol/gol.go - initiates the client and server communication
* gol/ticker.go - sends regular 'ticks' to the client to prompt events
* stubs/stubs.go - contains the RPC commands available on the server
* bench_test.go - runs benchmarks to test performance of the system

See `report.pdf` for more information on the project. See my GoLServer repository for the server-side engine code. See my GoLParallel repository for an alternative parallel version of the simulation.

### How to run

To run the Game of Life simulation, complete the following steps:

1. Start the server using the command `go run .` while in the GoLServer directory
1. Start the client using the same command while in the GoLClient directory
1. Use keypresses to control behaviour of the client:

's' = save current world 
| 'p' = pause/resume the simulation
| 'q' = quit the client without killing the server
| 'k' = kill the server and quit the client
