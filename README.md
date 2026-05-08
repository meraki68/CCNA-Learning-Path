# Day 17 of My 60-Day Network Engineering Challenge
Today was all about routing decisions and failover — how networks stay online even when things break.

This is where networking becomes resilient.

Here’s what I worked on:
-	Analyzed routing tables on multiple routers
-	Identified the dynamic routing protocol in use
-	Observed how routers choose paths to:
-	Internal server (SRV1)
-	External server (1.1.1.1)
-	Configured floating static routes as backup paths
-	Simulated a link failure
-	Verified automatic failover and connectivity

💡 Key Takeaways:
-	Routers choose the best path based on metrics/administrative distance
-	Floating static routes act as backup routes
-	They only activate when the primary route fails
-	Network resilience depends on proper failover design
  
⚠️ What stood out:
When the main link went down, traffic automatically rerouted — no manual intervention needed.

This is how real networks stay online 24/7.
