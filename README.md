🌐 4-Router WAN Network (RIP v2)
🛰️ Project Overview

This topology demonstrates a 4-Router WAN network connecting 4 different LAN segments, each with its own server.
Routers are connected using Serial WAN links, forming a redundant mesh topology.

🧩 Network Components

LAN 1 – 192.168.1.0 (Green Zone)

PCs, Laptop, Printer

DHCP/Fileserver

![Topology](images/topology.png)


Routers

Router0 (192.168.1.10) ![RIP Routing Config](rip-routing.png)


Router2 (192.168.2.20)![RIP Routing Config](rip-routing.png)


Router1 (192.168.3.30)![RIP Routing Config](rip-routing.png)


Router3 (192.168.4.40)![RIP Routing Config](rip-routing.png)


🔧 WAN Links (Serial)

All routers are connected in a full-mesh style using:

Se0/0/0

Se0/1/0

Se0/0/1

Se0/1/1

This provides redundancy and multi-path routing.

(Make sure each router has correct next-hop.)

![server1 to LAN2 Ping](ping-1.png)
![server2 to LAN3 Ping](ping-2.png)
![server3 to LAN4 Ping](ping-3.png)
![server4 Router Ping](ping-4.png)


WEB browser checking 
![Web Browser Checking](web-browser.png)
![Web Browser Checking](web-browser.png)


🎯 Summary

This project shows how to:

Build a multi-site WAN

Connect 4 different LAN networks

Use Serial WAN links

Configure Static routing

Test end-to-end connectivity


