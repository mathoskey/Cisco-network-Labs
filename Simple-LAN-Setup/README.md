Subject: Simple LAN Setup Steps - Packet Tracer Assignment

Body:

SIMPLE LAN SETUP - COMPLETE STEPS

Step 1: Add Devices

Router 4330

Switch 2960

Two PCs

Step 2: Connect Cables (Copper Straight-Through)

PC0 to Switch (FastEthernet0/1)

PC1 to Switch (FastEthernet0/2)

Switch to Router (Gig0/1 to Gig0/0/0)

Step 3: Configure Router

text
enable
configure terminal
interface gigabitEthernet 0/0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit
write memory
Step 4: Configure PC0

IP: 192.168.1.2

Subnet Mask: 255.255.255.0

Default Gateway: 192.168.1.1

DNS Server: 192.168.1.100

Step 5: Configure PC1

IP: 192.168.1.3

Subnet Mask: 255.255.255.0

Default Gateway: 192.168.1.1

DNS Server: 192.168.1.100

Step 6: Test Connectivity
From PC0: ping 192.168.1.1 and ping 192.168.1.3
From PC1: ping 192.168.1.1 and ping 192.168.1.2

Step 7: Save

Router: write memory

Packet Tracer: File → Save As → "simple LAN setup.pkt"
