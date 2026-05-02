# Day 11 of My 60-Day Network Engineering Challenge
Today, I leveled up from router-based VLAN routing to using a Multilayer Switch (Layer 3 switching).

This is how modern networks actually operate.

Here’s what I worked on:
-	Replaced router-on-a-stick with a Layer 3 point-to-point connection
-	Configured a default route on the multilayer switch
-	Created SVIs (Switch Virtual Interfaces) for each VLAN
-	Assigned gateway IPs directly on the switch
-	Tested inter-VLAN communication
-	Verified Internet connectivity (ping 1.1.1.1)

💡 Key Takeaways:
-	Multilayer switches can handle both switching and routing
-	SVIs act as gateways for VLANs
-	This design is faster and more scalable than router-on-a-stick
-	Default routes are essential for external connectivity

⚠️ What stood out:
Moving routing from the router to the switch simplifies the network and improves performance.
