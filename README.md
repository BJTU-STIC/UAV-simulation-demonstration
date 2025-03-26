# UAV-simulation-demonstration
This warehouse gives a UAV simulation video based on Omnet++ according to paper XXX.
## 1 Experimental parameter setting
The parameter Settings of this simulation experiment are given below.
### 1.1 Network-related parameters setting
| Name | Setting |
|:---------|:---------|
|Network configurator   | Ipv4NetworkConfigurator   |
| Arp   | GlobalArp   |
| Network Interface   | IEEE80211Interface   |
| Management layer   | IEEE80211MgmtAdhoc   |
| Bitrate   | 48 Mbps   |
| Transport layer protocol   | UDP   |
### 1.2 UAV-related parameters setting
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
### 1.3 Power-related parameters setting
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
## 2 The UAV simulation video
According to the parameter settings mentioned above, we conducted a simulation experiment based on Omnet++. Specifically, for LP2-CACKM with and without MAm, we simulate the process of JUAV joining the cluster. In practice, the process of JUAV joining a cluster is very rapid. Therefore, in order to show the whole process more clearly, we have slowed down the whole process by setting parameters.
### 2.1 LP2-CACKM with MAm
In the case of LP2-CACKM with MAm, we simulate the process of JUAV joining cluster in three stages. The first is the registration process of JUAV, which corresponds to steps 1-2 in Section IV.C of the paper. Below is the corresponding simulation gif. The simulation video can be found in [First stage](Simulation%20video/First%20stage--LP2-CACKM%20with%20MAm.mp4).

![First Stage Demo](Simulation%20gif/First%20stage--LP2-CACKM%20with%20MAm.gif)

The second stage is the authentication process of JUAV authenticity by CMs inside the cluster, which corresponds to steps 3-4 in Section IV. C of the paper. Below is the corresponding simulation video. The simulation video can be found in [Second stage](Simulation%20video/Second%20stage--LP2-CACKM%20with%20MAm.mp4).

![Second Stage Demo](Simulation%20gif/Second%20stage--LP2-CACKM%20with%20MAm.gif)

The third stage is the verification process of other CLS for CMs authentication results on the authenticity of JUAVs, corresponding to steps 5-7 in Section IV. C of the paper. Below is the corresponding simulation video. The simulation video can be found in [Third stage](Simulation%20video/Thrid%20stage--LP2-CACKM%20with%20MAm.mp4).

![Third Stage Demo](Simulation%20gif/Third%20stage--LP2-CACKM%20with%20MAm.gif)

### 2.2 LP2-CACKM without MAm
In the case of LP2-CACKM without MAm, since JUAVs' joining request and CMs' authentication result are sent continuously, we show the process of JUAV joining cluster through a video, which corresponds to steps 1-7 in Section IV.C of the paper. Below is the corresponding simulation video. The simulation video can be found in [LP2-CACKM without MAm](Simulation%20video/LP2-CACKM%20without%20MAm.mp4).

![Wihout MAm](Simulation%20gif/LP2-CACKM%20without%20MAm.gif)

