# Day 19 of My 60-Day Network Engineering Challenge
Today, I worked on one of the most important routing protocols in enterprise networking — OSPF (Open Shortest Path First) — and this lab helped me understand how dynamic routing actually behaves in a multi-router environment.

Here’s what I configured in today’s lab:
- Assigned hostnames and IP addresses to all routers
- Configured and enabled router interfaces
- Created loopback interfaces on each router for stable router IDs
- Enabled OSPF across the network topology
- Learned why certain interfaces should be configured as passive interfaces
- Avoided enabling OSPF on the Internet-facing link
- Configured R1 as an ASBR (Autonomous System Boundary Router)
- Advertised a default route into the OSPF domain
- Verified routing tables on R2, R3, and R4 to confirm route propagation

One major takeaway from today’s lab was understanding how a default route can be injected into an OSPF network and automatically learned by neighboring routers.

Seeing the routes populate dynamically made the entire concept feel much more real.



