# Day 8 of My 60-Day Network Engineering Challenge
Today was all about Subnetting + Routing — and this is where things got really interesting.

Starting with just 192.168.5.0/24, I had to design a network that supports multiple LANs with different host requirements.

Here’s what I worked on:
-	Subnetted a /24 network into multiple smaller networks
-	Allocated IP ranges based on host needs (VLSM)
- Assigned:
- First usable IP → PCs
- Last usable IP → Router interfaces
-	Configured static routes between routers
-	Verified full connectivity across all LANs

💡 Key Takeaways:
-	Subnetting is about efficient IP allocation, not just splitting networks
-	Different LAN sizes require different subnet masks (VLSM)
-	Planning is everything — one mistake affects the entire network
-	Routing connects all subnets into one functional network
  
⚠️ What challenged me:
Designing subnets that fit each LAN without wasting IP space.

This felt like designing a real enterprise network.
