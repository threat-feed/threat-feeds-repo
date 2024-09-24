**THREAT FEED / EXTERNAL DYNAMIC LIST**

This list includes the IP addresses which are trying to log in to your SSLVPN or your firewall/router interface. The IP addresses are collected from private source and are updated weekly.

**Implementation**

FORTIGATE:
--------
Security Fabric -> External connectors -> Create New -> Threat Feeds > IP Address -> URI of external resource: **https://raw.githubusercontent.com/threat-feed/threat-feeds-repo/main/IP_Threat_Feed.txt**
