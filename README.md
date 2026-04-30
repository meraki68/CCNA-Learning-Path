# Day 9 of My 60-Day Network Engineering Challenge
Today, I stepped into VLANs and network segmentation — a core concept in real-world networks.

Instead of one flat network, I divided it into multiple logical networks:
-	Engineering
-	HR
-	Sales

Here’s what I worked on:
-	Configured IP addressing for each VLAN
-	Set default gateways using the last usable IP
-	Connected router to switch using multiple interfaces
-	Assigned switch ports to the correct VLANs
-	Tested communication between devices
-	Observed broadcast behavior using simulation mode

💡 Key Takeaways:
-	VLANs logically separate networks even on the same physical switch
-	Devices in different VLANs cannot communicate without routing
-	Each VLAN acts like its own network (own broadcast domain)
-	Broadcast traffic stays within the same VLAN

⚠️ What stood out:
Sending a broadcast ping showed exactly how traffic is isolated within VLANs — super powerful concept.

This is how real organizations separate departments securely.
