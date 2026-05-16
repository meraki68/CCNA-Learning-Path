# Day 25 of My 60-Day Network Engineering Challenge
Today’s lab pushed my understanding of IPv6 even further — especially around automatic addressing and routing redundancy.

This wasn’t just about configuring routers.

It was about understanding how modern IPv6 networks can intelligently configure themselves and maintain backup connectivity paths.

What I worked on today:
- Enabled IPv6 routing on all routers
- Used SLAAC (Stateless Address Autoconfiguration) to automatically assign IPv6 addresses to PCs
- Verified the IPv6 addresses generated on each host
- Configured IPv6 static routes between routers
- Implemented a backup routing path through R2 for redundancy
- Tested end-to-end IPv6 connectivity between PC1 and PC2

One of the most interesting parts of today’s lab was seeing SLAAC in action.

Instead of manually assigning addresses, the PCs automatically generated their own IPv6 addresses using router advertisements — which really demonstrates the scalability and automation advantages of IPv6.
Another key lesson was configuring a backup path.

Learning how to create primary and secondary routing behavior gave me a better understanding of network resilience and failover design.

IPv6 is designed not just for more devices, but for smarter and more automated networking.

