# Day 10 of My 60-Day Network Engineering Challenge
Today, I connected everything together using Trunking + Router-on-a-Stick.

This is how multiple VLANs communicate in real networks.

Here’s what I worked on:
- Configured switch ports as access ports for different VLANs
-	Set up a trunk link between switches (carrying multiple VLANs)
-	Configured a native VLAN for untagged traffic
-	Implemented router-on-a-stick for inter-VLAN routing
-	Assigned gateway IPs to router subinterfaces
-	Tested full connectivity across all VLANs

💡 Key Takeaways:
-	Access ports belong to a single VLAN
-	Trunk ports carry multiple VLANs using tagging
-	Native VLAN handles untagged traffic
-	Router-on-a-stick enables communication between VLANs

⚠️ What stood out:
Without router-on-a-stick, VLANs are isolated — with it, the network becomes fully connected.

This felt like building a real enterprise network setup.
