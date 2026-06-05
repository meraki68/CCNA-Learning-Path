# Day 40 of 60 — Dynamic ARP Inspection: Closing the Door on ARP Poisoning
If DHCP Snooping is the lock on the front door, Dynamic ARP Inspection is the security camera watching every conversation inside.

What I configured:
- R1 as DHCP server for 192.168.1.0/24
   - (Excluded .1 – .9 for infrastructure, default gateway: R1)
- DHCP Snooping on SW1 and SW2
  - (Builds the binding table DAI depends on)
- DAI on SW1 and SW2:
  - Enabled all additional validation checks (src-mac, dst-mac, IP)
  - Trusted ports configured on router and switch uplinks
  
And just like DHCP Snooping, trust is explicit:
Uplinks to routers and switches are trusted — everything else is untrusted by default.

