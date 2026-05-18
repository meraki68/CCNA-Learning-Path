# Day 27 of My 60-Day Network Engineering Challenge
Today’s lab took network security a step further with Extended ACLs — where traffic filtering becomes much more detailed and powerful.

Unlike standard ACLs that mainly filter based on source addresses, today I worked on controlling traffic based on specific hosts, protocols, and services.
This felt much closer to real-world enterprise security implementation.

What I worked on today:
- Configured Extended ACLs on Cisco routers
- Restricted communication between specific networks and hosts
- Blocked DNS access to a server from selected subnets
- Prevented access to HTTP and HTTPS services on a server
- Tested permitted vs denied traffic behavior
- Strengthened understanding of protocol-based traffic filtering

Policies implemented in the lab:
- Hosts in 172.16.2.0/24 were blocked from communicating with PC1
- Hosts in 172.16.1.0/24 were denied access to the DNS service on SRV1
- Hosts in 172.16.2.0/24 were denied access to HTTP and HTTPS services on SRV2

Instead of blocking an entire network completely, you can selectively control which services users are allowed to access — which is exactly how organizations enforce security policies in production environments.

Network security is not just about blocking traffic — it’s about allowing the right traffic while denying unauthorized access.

