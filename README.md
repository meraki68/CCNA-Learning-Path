# Day 1 of My 60-Day Network Engineering Challenge

Today, I focused on basic device configuration & security using Cisco CLI.

Here’s what I worked on:
-	Changed device hostnames (R1, SW1)
-	Configured enable password and tested access
-	Enabled password encryption
-	Implemented a more secure enable secret
-	Verified encryption types in the running configuration
-	Saved configurations properly

💡 Key Takeaways:
- enable secret is more secure than enable password
-	Password encryption prevents configs from being easily exposed
-	Cisco uses different encryption types:
-	Type 7 → weak (reversible)
-	Type 5 → strong (MD5 hashed)

⚠️ One thing that stood out:

Even after setting both passwords, the device prioritizes enable secret for authentication.

