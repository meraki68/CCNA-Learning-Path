# Day 14 of My 60-Day Network Engineering Challenge
Today, I went deeper into Spanning Tree Protocol (STP) — not just understanding it, but controlling it.

Instead of letting the network decide everything automatically, I learned how to influence STP behavior.

Here’s what I worked on:
-	Analyzed the current STP topology using CLI
-	Identified root bridge and port roles
-	Configured primary and secondary root bridges per VLAN
-	Tuned STP using:
-	Path cost
-	Port priority
-	Observed how changes affected root port selection
-	Configured PortFast + BPDU Guard for edge port security

💡 Key Takeaways:
-	STP can be manually optimized for better network design
-	Root bridge placement is critical for performance
-	Cost and priority influence path selection
-	PortFast speeds up host connectivity
-	BPDU Guard protects against misconfigurations

⚠️ What stood out:
Small changes in cost or priority can completely change traffic flow.

This is where networking shifts from learning → engineering decisions.
