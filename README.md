# DDoS_Attack_Sequence.md
By Brandon Norris

#### DDOS Attack Steps
#####	1. The attacker first assembles a botnet, which is a network of computers under their control. This can be done by using their own systems or by infecting other users’ devices with malware to gain remote access. 
#####	2. Once the botnet is in place, the attacker launches the Distributed Denial of Service (DDoS) attack. This involves flooding the target web server with a massive number of simultaneous connection requests. The goal is to overwhelm the server’s resources, preventing legitimate users from accessing it. Without proper defenses, the server can become unresponsive or crash entirely under the load.
#####	3.Detecting and stopping a DDoS attack can be challenging, especially since high traffic isn’t always suspicious—businesses often want more visitors. In many cases, the first step in mitigation may be to temporarily take the server offline to assess and respond to the threat.
######	However, several proactive security measures can help:
	* Firewall Configuration: Firewalls can be set to block known malicious IP ranges and filter out traffic on unused or suspicious ports.
	* Intelligent Firewalls: Advanced firewalls like Cisco’s Adaptive Security Appliance (ASA) can leverage AI and behavioral analysis to detect and stop DDoS attacks in real-time by analyzing incoming traffic patterns and identifying botnet behavior.



```mermaid
sequenceDiagram
Actor Attacker
Actor GeneralUser
participant BotNet
participant WebServer

Attacker->>BotNet: 1. The attacker first assembles a botnet.
BotNet->>WebServer: 2. Attacker launches the DDOS Attack with their BotNet.
Note right of WebServer: Becomes Unresponsive.
GeneralUser--xWebServer: 3. Unable to access the Web Services, due to the DDOS attack.
```

```mermaid
sequenceDiagram
actor Attacker
actor GeneralUser
participant BotNet
participant Firewall
participant WebServer

Attacker->>BotNet: 1. The attacker first assembles a botnet.
BotNet-xFirewall: 2. Attacker launches the DDOS Attack with their BotNet.
GeneralUser-->>Firewall: 3. The user's network traffic is analyze to be legit.
Firewall-->>WebServer: 4. The User's traffic is allowed.
WebServer-->>GeneralUser: 
```
