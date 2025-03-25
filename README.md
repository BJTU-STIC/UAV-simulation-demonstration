# UAV-simulation-demonstration
This warehouse gives a UAV simulation video based on Omnet++ according to paper XXX.
## Experimental parameter setting
The parameter Settings of this simulation experiment are given below.
### Network-related parameters setting
| Name | Setting |
|:---------|:---------|
|Network configurator   | Ipv4NetworkConfigurator   |
| Arp   | GlobalArp   |
| Network Interface   | IEEE80211Interface   |
| Management layer   | IEEE80211MgmtAdhoc   |
| Bitrate   | 48 Mbps   |
| Transport layer protocol   | UDP   |
### UAV-related parameters setting
| Name | Setting |
|:---------|:---------|
|Physical layer modules   | IEEE80211ScalarRadio   |
| Transmitter power   | 500 mW   |
| Receiver sensitivity   | -85 dBm   |
| Receiver energy detection   | -85 dBm   |
| Mobility module   | Linear movement   |
| Mobility speed   | 100 m/s   |
| Constraint area   | 100 m/s   |
| N_JUAV   | 3   |
| N_CM   | 4   |
| N_CL   | 4   |
### Power-related parameters setting
| Name | Setting |
|:---------|:---------|
|Power consumption model   | StateBasedEpEnergyConsumer   |
| Sleep power consumption   | 0 mW  |
| Receiver idle power consumption   | 2 mW   |
| Receiver busy power consumption   | 5 mW   |
| Receiver receiving power consumption   | 100 mW   |
| Transmitter idle power consumption   | 2 mW   |
| Transmitter transmitting power consumption   | 300 mW   |
| UAV initial energy   | 0.01 J   |
## The UAV simulation video
The parameter Settings of this simulation experiment are given below.

