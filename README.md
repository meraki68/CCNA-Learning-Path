# Day 7 of My 60-Day Network Engineering Challenge
Today, I went deeper into how data actually moves across a network — at the MAC address level.

Not just IPs… but what’s happening behind the scenes.

Here’s what I worked on:
-	Traced packets from PC1 → PC4 across multiple routers
-	Identified source & destination MAC addresses at each hop
-	Observed how MAC addresses change at every segment
-	Used Packet Tracer simulation mode to visualize traffic
-	Verified ARP and MAC learning before analysis

💡 Key Takeaways:
-	MAC addresses change at every hop, but IP addresses stay the same
-	Each router rewrites the Layer 2 (MAC) header
-	Switches forward frames based on MAC tables
-	ARP is essential before communication begins

⚠️ What stood out:
Even though the packet travels end-to-end, each segment behaves like a separate conversation.

This is where networking starts to really click.

From IP logic → to actual frame movement.

