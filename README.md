# Day 20 of My 60-Day Network Engineering Challenge
Today’s lab was centered around OSPF configuration, routing optimization, and understanding how routers establish neighbor relationships behind the scenes.

This wasn’t just about enabling a routing protocol… it was about understanding how routers communicate, exchange routes, and make forwarding decisions dynamically.

Here’s what I worked on today:
- Configured hostnames and IP addressing across routers
- Enabled and verified router interfaces
- Configured loopback interfaces for stable router identification
- Enabled OSPF directly on router interfaces
- Configured passive interfaces where appropriate
- Tuned OSPF reference bandwidth so FastEthernet interfaces use a cost of 100
- Configured R1 as an ASBR to advertise a default route into the OSPF domain
- Verified routing tables and analyzed learned default routes
- Used Simulation Mode to inspect OSPF Hello packets and neighbor formation

💡 Key Takeaways:
- OSPF dynamically builds neighbor relationships using Hello packets
- Loopback interfaces help maintain consistent Router IDs
- Passive interfaces improve security and reduce unnecessary updates
- Reference bandwidth tuning ensures more accurate path selection
- ASBRs can inject external/default routes into an OSPF domain

⚠️ What stood out:
Seeing the OSPF Hello process in Simulation Mode made the protocol feel much more real. Understanding the fields exchanged between routers gave me a clearer picture of how adjacencies are formed and maintained.

Today reinforced an important lesson:
Networking becomes easier when you understand the behavior of protocols — not just the commands.
