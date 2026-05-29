# Day 36 of 60 — Dynamic NAT vs PAT: One Lab That Shows You Everything
Dynamic NAT and PAT are how the real internet actually works for most networks — and today's lab exposed exactly WHY one is limiting and the other is essential.

What i did
— Dynamic NAT on R1:
- Defined inside/outside interfaces
- Created an ACL to match all 172.16.0.0/24 traffic
- Built a NAT pool: only 2 public IPs available (100.0.0.1 – 100.0.0.2)
- PC1 and PC2 pinged google.com successfully ✅

Then PC3 tried to ping google.com.

And failed. ❌

Why? The pool was exhausted. 2 public IPs. 2 already in use. PC3 had no address to borrow — it simply got dropped.

That's the hard limit of dynamic NAT in a single sentence:
More devices than public IPs = some devices go dark.

The Switched to PAT (NAT Overload):
- Cleared the NAT table
- Removed the pool-based config
- Reconfigured using R1's single public IP with overload

Now ALL three PCs pinged google.com successfully ✅✅✅

Checked the NAT translation table on R1 — same public IP, three different source port numbers. That's PAT in action: one IP address, thousands of simultaneous sessions, each tracked by port.

This is exactly how your home router works right now.
And how ISPs handle millions of subscribers behind shared public IPs.

The difference between Dynamic NAT and PAT isn't just config syntax — it's a fundamental shift in how you think about address scalability.

