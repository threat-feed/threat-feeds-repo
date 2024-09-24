# **THREAT FEED / EXTERNAL DYNAMIC LIST**

This list includes the IP addresses of bots which are trying to log in to your SSLVPN or your firewall/router interface. The IP addresses are collected from private source and are updated weekly.

## **Implementation:**

### FORTIGATE
Security Fabric -> External connectors -> Create New -> Threat Feeds > IP Address -> URI of external resource: **https://raw.githubusercontent.com/threat-feed/threat-feeds-repo/main/IP_Threat_Feed.txt**

If you have MGMT and SSLVPN on a loopback interface use this list as a source in security policy which denies access to VIP.
If you don’t have SSLVPN on a loopback interface, you can also use it in SSLVPN settings to deny them to connect to VPN but they will still be able to reach your public facing interface.

### PALO ALTO
Objects -> External Dynamic Lists -> Add -> Type: IP List -> Source: **https://raw.githubusercontent.com/threat-feed/threat-feeds-repo/main/IP_Threat_Feed.txt**
