# Day 40 of 60 — DHCP Snooping: The Feature That Stops Rogue DHCP Attacks Dead

Imagine a malicious device on your network handing out fake IP addresses to every PC that boots up.
Wrong gateway. Wrong DNS. Every user silently redirected through an attacker's machine.

That's a rogue DHCP attack — and it's trivially easy to execute on an unsecured network.

Today's lab was about stopping it cold with DHCP Snooping.

What I built and configured:
- Set up R1 as the DHCP server for 192.168.1.0/24
- Excluded 192.168.1.1 – 192.168.1.9 from the pool (reserved for infrastructure)
- Enabled DHCP snooping on SW1 and SW2
- Configured uplink interfaces as trusted ports


