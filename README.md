🌐 4-Router WAN Network (RIP v2)
📌 Overview

Mini WAN loyihasi:

4 ta router (Full-Mesh)

4 ta server (DHCP, DNS, Web1, Web2)

1 ta LAN (PC, Laptop, Printer)

RIP v2 routing
Cisco Packet Tracerda qurilgan va test qilingan.

📸 Topology Screenshot:

🖼️ [ INSERT TOPOLOGY IMAGE ]

🖧 Devices
🔹 Routers
Router	IP
R2	192.168.1.10
R3	192.168.4.40
R0	192.168.2.20
R1	192.168.3.30
🖼️ [ ROUTERS SCREENSHOT ]

🗄️ Servers
Server	Service	IP
Server0	DHCP	Auto
Server1	Web	192.168.2.21
Server2	Web	192.168.3.31
Server3	DNS	192.168.4.41
🖼️ [ SERVERS SCREENSHOT ]

⚙️ Routing (RIP v2)
router rip
 version 2
 network 192.168.1.0
 network 192.168.2.0
 network 192.168.3.0
 network 192.168.4.0
 no auto-summary

🖼️ [ RIP CONFIG SCREENSHOT ]

📡 Connectivity Tests
🏓 Ping
ping 192.168.2.21
ping 192.168.3.31
ping 192.168.4.41

🖼️ [ PING SCREENSHOT ]

🌐 Web Browser
http://192.168.2.21
http://192.168.3.31

🖼️ [ WEB TEST SCREENSHOT ]

✅ Result

✔ Routing ishladi
✔ Barcha serverlar ping bo‘ladi
✔ Web serverlar ochildi
✔ LAN → WAN to‘liq ishladi

🖼️ [ SUCCESS SCREENSHOT ]
