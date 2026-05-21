# Day 29 of My 60-Day Network Engineering Challenge
Today’s lab focused on something that’s often overlooked in networking — time synchronization.

What I worked on today:
- Configured the software clock on multiple routers
- Set router time zones to match local time
- Configured R1 to synchronize with an external NTP server over the Internet
- Verified NTP stratum levels
- Configured R1 as a Stratum 8 NTP master
- Enabled authenticated NTP synchronization between routers
- Configured hardware calendar updates through NTP
- Worked with preconfigured OSPF connectivity

Seeing routers synchronize time across the network really highlighted how important consistency is in infrastructure environments.

Another interesting part was implementing NTP authentication, which helps ensure devices only trust valid time sources — an important security best practice.

Reliable networks depend on accurate time.


