# Day 16 of My 60-Day Network Engineering Challenge
Today was all about EtherChannel — combining multiple links into one logical connection for better performance and redundancy.

This is how real networks handle high traffic efficiently.

Here’s what I worked on:
-	Configured Layer 2 EtherChannel (LACP) between access and distribution switches
-	Configured Layer 2 EtherChannel (PAgP) on another link
-	Built a Layer 3 EtherChannel between distribution switches
-	Configured routing for end-to-end connectivity
-	Analyzed default load-balancing behavior
-	Tuned load balancing to use source + destination IP

💡 Key Takeaways:
-	EtherChannel increases bandwidth + redundancy
-	LACP (open standard) vs PAgP (Cisco proprietary)
-	Multiple physical links act as one logical link
-	Load balancing determines how traffic is distributed

⚠️ What stood out:
Without proper load balancing, traffic may not use all available links efficiently.

This is how networks scale under heavy traffic.

