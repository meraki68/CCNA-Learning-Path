# Day 42 of 60 — HSRP + STP: When Gateway Redundancy and Loop Prevention Must Work Together
Today's lab was about making HSRP and STP work in harmony — not against each other

What I configured:
- VLAN 10 (10.0.10.0/24):
    - DSW1 = HSRP Active + STP Root
    - DSW2 = HSRP Standby + STP Secondary Root
    - Traffic flows through DSW1. STP keeps that path open. Perfect alignment.

- VLAN 20 (10.0.20.0/24):
    - DSW2 = HSRP Active + STP Root
    - DSW1 = HSRP Standby + STP Secondary Root
    - Traffic flows through DSW2. STP keeps that path open. Same logic, opposite switch.

This is exactly how enterprise and ISP distribution layers are designed in production. Two switches. Two VLANs. Symmetric redundancy. No single point of failure.

The key insight: HSRP and STP solve different problems, but they must be configured with the same intent — or they'll fight each other silently while your users file tickets.



