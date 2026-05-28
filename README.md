# Day 35 of 60 — The Moment Private IPs Meet the Internet (Static NAT Deep Dive)

Before today's config: PC1 tries to ping 8.8.8.8.
Result? Nothing. Dead silence.

That's the reality of private IP addressing — 172.16.0.0/24 means absolutely nothing to the public internet. Without NAT, your internal network is invisible.

Today's lab fixed that.

What I configured on R1:
- Identified and tagged the inside interface (G0/1 — LAN side)
- Identified and tagged the outside interface (G0/0 — toward the internet)
- Created static NAT entries mapping each PC's private IP to a dedicated public address in the 100.0.0.x/24 range

After NAT was in place:
- PC1 pinged 8.8.8.8 successfully ✅
- All three PCs resolved and pinged google.com
- Ran 'show ip nat translations' on R1 — watched the inside local vs inside global mappings appear in real time


