🌐 4-Router WAN Network (RIP v2)
🛰️ Project Overview

This topology demonstrates a 4-Router WAN network connecting 4 different LAN segments, each with its own server.
Routers are connected using Serial WAN links, forming a redundant mesh topology.

🧩 Network Components

LAN 1 – 192.168.1.0 (Green Zone)

PCs, Laptop, Printer

DHCP/Fileserver

![Topology]<img width="1922" height="1020" alt="Screenshot 2025-12-23 191752" src="https://github.com/user-attachments/assets/ac6a6d49-a5b8-48f8-9627-7fea2f1a4319" />



Routers

Router0 (192.168.1.10) <img width="1923" height="871" alt="Screenshot 2025-12-23 221002" src="https://github.com/user-attachments/assets/42cd7ad0-7707-45c5-a17f-540f08c989c0" />



Router2 (192.168.2.20)<img width="1923" height="882" alt="Screenshot 2025-12-23 220951" src="https://github.com/user-attachments/assets/15863364-375b-4d51-befc-9adad1146577" />



Router1 (192.168.3.30)<img width="1904" height="843" alt="Screenshot 2025-12-23 220938" src="https://github.com/user-attachments/assets/7dd95fc0-73f7-4f7a-b9fd-b76132581c4a" />



Router3 (192.168.4.40)<img width="1874" height="895" alt="Screenshot 2025-12-23 220920" src="https://github.com/user-attachments/assets/1bfd6a26-0357-4ed0-a87d-cddf015de850" />



🔧 WAN Links (Serial)

All routers are connected in a full-mesh style using:

Se0/0/0

Se0/1/0

Se0/0/1

Se0/1/1

This provides redundancy and multi-path routing.

(Make sure each router has correct next-hop.)

![server1 to LAN2 Ping](ping-1.png<img width="1884" height="861" alt="Screenshot 2025-12-23 221643" src="https://github.com/user-attachments/assets/a5f92b0e-2e6e-4c5a-a37c-351bb2b1711a" />
)
![server2 to LAN3 Ping]<img width="1884" height="861" alt="Screenshot 2025-12-23 221643" src="https://github.com/user-attachments/assets/275d0582-52d1-4234-91d2-247f7d877649" />

![server3 to LAN4 Ping]<img width="1923" height="840" alt="Screenshot 2025-12-23 221107" src="https://github.com/user-attachments/assets/3df31d02-a2ff-4e65-9c99-eeb031fdc1cb" />

![server4 Router Ping]<img width="1874" height="895" alt="Screenshot 2025-12-23 220920" src="https://github.com/user-attachments/assets/bd0d010d-b28b-4fb1-8fb8-a48f586b2fd5" />



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


