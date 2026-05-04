# Day 13 of My 60-Day Network Engineering Challenge
Today, I dived into Spanning Tree Protocol (STP) — the protocol that prevents network loops.

At first glance, the topology looked fine…
But underneath, STP was making decisions on which links to block and which to forward.

Here’s what I worked on:
-	Identified the root bridge in the network
-	Analyzed switch priorities and MAC addresses
-	Determined port roles:
-	Root ports
-	Designated ports
-	Non-designated (blocked) ports
-	Verified everything using CLI commands

💡 Key Takeaways:
-	STP prevents loops by blocking redundant paths
-	The switch with the lowest Bridge ID becomes the root bridge
-	Each port is assigned a role based on the best path to the root
-	Redundant links are good — but must be controlled

⚠️ What stood out:
Even though multiple paths exist, only one is active — the rest are kept as backups.

This is how networks stay stable even with redundancy.
