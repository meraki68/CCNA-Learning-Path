# Day 37 of 60 — When Data and Voice Share the Same Wire (ROAS + Voice VLANs)
Today's lab introduced one of the most practically relevant concepts I've hit in this challenge — Router on a Stick (ROAS) combined with Voice VLANs. The kind of setup you'd actually find in an office or small ISP customer site.

What I configured:

- Assigned SW1's interfaces to the correct VLANs
  → VLAN10 (192.168.10.0/24) for data — PC1 and PC2
  → VLAN20 (192.168.20.0/24) for voice — PH1 and PH2
- Configured ROAS on the SW1–R1 link
  → Single physical trunk link carrying multiple VLANs
  → Subinterfaces on R1 handling inter-VLAN routing

ROAS makes all of this possible over a single uplink — no need for a dedicated router interface per VLAN. It's elegant, efficient, and widely deployed.

Understanding how voice and data coexist on the same physical infrastructure is a skill that goes beyond CCNA — it's what network engineers deal with every day in the field.


