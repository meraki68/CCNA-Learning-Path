# Day 34 of 60 — Securing a Brand New Switch from Scratch

A freshly added switch is one of the most vulnerable devices on a network.
No hostname. No credentials. No remote access policy. Just a blank slate waiting to be exploited.

Today's lab task was exactly that scenario — SW2 just landed in the network, and it was my job to lock it down before it became a liability.

Here's what I configured:
- Console Access (via Laptop1)
- Set the hostname and enable secret
- Created a local user account (username + password)
- Assigned VLAN1 SVI: 192.168.2.253/24
- Set the default gateway to R2
- Authentication: Local user only
- Exec timeout: 5 minutes (auto-logout on idle)

 SSH Remote Access Hardening
- Domain name configured for RSA key generation
- RSA key size: 2048 bits (the minimum you should accept in production)
- Authentication: Local user
- Exec timeout: 5 minutes
- Protocols: SSH only — Telnet disabled entirely
- Access restricted to PC1 ONLY via ACL

That last point is the one most people skip in labs but matters most in real ISP environments — limiting WHO can even attempt to reach your management plane.

Every switch that hits your rack should go through a checklist like this before it ever touches production traffic.




