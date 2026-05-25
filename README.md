# Day 33 of My 60-Day Network Engineering Challenge
Today’s lab focused on logging and syslog, reinforcing how critical proper logging is for visibility and troubleshooting in networks.

What I worked on today:
- Connected to R1’s console via PC2 and toggled interface **G0/0** (`shutdown` / `no shutdown`) to generate syslog messages.
- Observed and identified the **syslog severity level** reported when the interface went down/up.
- Enabled timestamps on log messages (`service timestamps log datetime msec`) to accurately record when events occur.
- Initiated a Telnet session from PC1 to R1’s **G0/0** and enabled the unused **G0/1** interface to test remote session behavior.
- Noted that, by default, VTY lines don’t display console logs (Packet Tracer has `logging monitor` on by default, so no extra command needed).
- Configured logging to R1’s internal **buffer** (size 8192 bytes) and set the severity to **debug**.
- Directed log messages to the external **Syslog server (SRV1)** with the command `logging host 192.168.1.100 debugging`.
- Verified that messages appear on the console, in the buffer, and on the central Syslog server.

This lab reinforced that proactive monitoring through logging is essential for network reliability. 

