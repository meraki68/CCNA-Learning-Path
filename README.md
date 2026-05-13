# Day 22 of My 60-Day Network Engineering Challenge
Today’s lab was all about HSRP (Hot Standby Router Protocol) and understanding how network redundancy keeps users connected even when a router fails.

This was one of the most practical labs I’ve done so far because it simulated a real-world high availability setup used in enterprise environments.

Here’s what I worked on today:
- Tested connectivity to an external server (8.8.8.8)
- Configured HSRPv2 on R1 and R2
- Adjusted router priorities to control the active and standby routers
- Enabled preemption so the preferred router can reclaim active status
- Configured a Virtual IP (VIP) as the default gateway for end devices
- Verified ARP table mappings to observe the virtual MAC address behavior
- Simulated router failure by shutting down R1
- Confirmed failover to R2 without losing connectivity
- Powered R1 back on and verified automatic recovery/preemption

One of the biggest lessons from today was seeing how seamless failover works in a redundant network design.

Even when the primary router went down, connectivity continued because the standby router immediately took over.

This lab strengthened my understanding of:
🔹 First Hop Redundancy Protocols (FHRP)
🔹 Gateway redundancy
🔹 High availability design
🔹 Network resilience
🔹 Failover and recovery mechanisms
🔹 Real-world enterprise networking concepts
Networking is becoming more exciting the deeper I go into these labs because every concept connects directly to how modern infrastructures stay reliable.

