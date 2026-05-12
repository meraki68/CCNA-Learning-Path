# Day 21 of My 60-Day Network Engineering Challenge
Today’s lab focused on troubleshooting and optimizing OSPF in a multi-router environment — and this one felt like a real-world network support scenario.

This wasn’t just about configuration… it was about identifying routing problems, understanding OSPF behavior, and fixing broken communication across the network.

Here’s what I worked on:
- Configured a new serial connection between R1 and R2
- Applied clock rate settings and enabled OSPF on the new link
- Investigated why only R3 had a route to 10.0.2.0/24
- Troubleshot OSPF neighbor adjacency issues between R2, R4, and R5
- Diagnosed why PCs could not reach the external server (8.8.8.8)
- Examined the OSPF LSDB to identify the LSAs present in the network

💡 Key Takeaways:
- OSPF neighbor relationships must match correctly for routes to propagate
- Small configuration mismatches can break adjacency formation
- Troubleshooting routing issues requires checking interfaces, OSPF configs, and LSDB information together
- External connectivity depends heavily on proper route advertisement and default routing
- Understanding LSAs gives deeper visibility into how OSPF shares topology information

⚠️ What stood out:
Today showed me that troubleshooting is where real learning happens.

It’s one thing to configure OSPF, but it’s another thing entirely to diagnose why routers refuse to become neighbors or why routes fail to appear.

Networking is starting to feel less like memorizing commands and more like solving logical puzzles.
