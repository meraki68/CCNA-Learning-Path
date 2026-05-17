# Day 26 of My 60-Day Network Engineering Challenge
Today’s lab was all about combining routing with network security policies — and it felt much closer to how real enterprise networks are designed.

This wasn’t just about getting devices connected.

It was about controlling who can communicate across the network and enforcing access policies using ACLs.
What I worked on today:
- Configured OSPF between R1 and R2 for full network connectivity
- Advertised multiple networks using dynamic routing
- Configured standard numbered ACLs on R1
- Configured standard named ACLs on R2
- Implemented traffic restrictions based on specific security requirements
- Verified connectivity and tested denied traffic scenarios

   Network policies implemented:
- Only PC1 and PC3 were allowed to access the 192.168.1.0/24 network
- Hosts in 172.16.2.0/24 were denied access to 192.168.2.0/24
- Communication between 172.16.1.0/24 and 172.16.2.0/24 was restricted in both directions

One major lesson from today was realizing that routing alone is not enough in networking.
A network can be fully connected, but without proper access control, security risks increase dramatically.

Good networking is not just about connectivity — it’s also about control, security, and intentional traffic design.
Every lab is helping me understand how real-world enterprise networks are built and protected.
