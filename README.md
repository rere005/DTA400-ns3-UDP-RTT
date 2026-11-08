# DTA400 — UDP Echo RTT Simulation

This project investigates how link delay affects UDP Echo round-trip time (RTT) using ns-3.45.

The simulation is adapted from the ns-3 tutorial example `first.cc`.

**Simulation settings**
- Two connected nodes
- Link bandwidth: 5 Mbps
- Packet size: 1024 bytes
- Number of packets: 10
- Sending interval: 1 second
- Tested link delays: 1 ms, 5 ms and 10 ms

**How to run**

Copy `udp_rtt.cc` into the `scratch` folder of ns-3.45. From the ns-3 directory, run `./ns3 run scratch/udp_rtt`.

To reproduce all three experiments, change the `Delay` setting to `1ms`, `5ms` and `10ms`, running the simulation after each change.

**Experimental results**

| Link delay | Average RTT | Received packets |
|---|---|---|
| 1 ms | 5.376 ms | 10/10 |
| 5 ms | 13.376 ms | 10/10 |
| 10 ms | 23.376 ms | 10/10 |

These results were obtained from ns-3.45 simulation runs.
