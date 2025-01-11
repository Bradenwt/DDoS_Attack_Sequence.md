mermaid
sequenceDiagram
participant Attacker->>Command to iniate attack 
participant BotNet->>WebServer: send multiple request 
participant WebServer->>Foward Incoming traffic
participant Firewall: Analyze Traffic patterns
Alt High traffic dectected
Firewall->>webServer: Allow traffic
end
Some what debreif of me trying to explain the sequence.The attacker is the individual initiating the attack on the host system,Botnet helps carry out the attack with the attacker,While the webserver is the target of the attack, the firewall repersents the networks defence system, and also monitors incoming and outcoming traffic.It all starts when the attacker sends the command to the botnet to flood the server,which floods the webserver with multiple request making it overload the webserver with too much request, then the firewall gets the oncoming request for analysis.
The Firewall is cruical when it comes to analyzing traffic pattern whether the patterns are legit or an attack.When the Firewall dectects high amounts of traffic it triggers defensive measures that block suspisous IP adresses associated with the Botnet and drops packets from the attacker, migaiting the attcker. The only way to bypass is if the Firewall detects noraml traffic and is deemed noraml and will allow it to pass through.
