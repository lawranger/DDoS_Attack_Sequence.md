# DDoS_Attack_Sequence.md
DDoS_Attack_Sequence.md

#### DDOS Attack Steps
#####	1. The attacker first assembles a botnet, which is a network of computers under their control. This can be done by using their own systems or by infecting other users’ devices with malware to gain remote access. 
#####	2. Once the botnet is in place, the attacker launches the Distributed Denial of Service DDoS attack. This involves flooding the target web server with a massive number of simultaneous connection requests. The goal is to overwhelm the server’s resources, preventing legitimate users from accessing it. Without proper defenses, the server can become unresponsive or crash entirely under the load.
```mermaid
sequenceDiagram
Actor Attacker
participant BotNet
Attacker->>BotNet: 1. The attacker first assembles a botnet.
participant WebServer
BotNet->>WebServer 2. Attacker launches the DDOS Attack
participant Firewall
```
