# 12 of My 60-Day Network Engineering Challenge
Today was all about VTP (VLAN Trunking Protocol) and trunking behavior — and it changed how I see VLAN management.

Instead of configuring VLANs on every switch manually, I explored how switches can share VLAN information automatically.

Here’s what I worked on:
-	Configured trunk links between switches
-	Disabled DTP for better control
-	Set up VTP modes:
-	Server (SW1)
-	Transparent (SW2)
- Client (SW3)
-	Created and tested VLAN propagation across switches
-	Configured access ports for end devices

💡 Key Takeaways:
-	VTP Server → creates and distributes VLANs
-	VTP Client → receives VLANs but cannot create
-	VTP Transparent → does NOT participate, only forwards
-	DTP can automatically form trunks (but disabling it gives more control)
  
⚠️ What stood out:
Changes made on one switch can automatically affect others — powerful, but risky if misconfigured.

This is where network management becomes centralized.
