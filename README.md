# Day 38 of 60 — Port Security: What Happens When an Unauthorised Device Plugs In?

Your switch doesn't care who plugs in by default. Any device. Any port. Full network access.

That's a serious problem in any production environment — and today's lab was all about fixing it with port security.

What I configured:
- SW1 — Interfaces F0/1, F0/2, F0/3:
• Violation mode: Shutdown
• Maximum MAC addresses: 1 per port
• Sticky learning: Disabled
• Aging time: 1 hour

One device per port. No exceptions. If a second MAC address shows up — the port shuts down immediately and goes into err-disabled state.

- SW2 — Interface G0/1:
• Violation mode: Restrict
• Maximum MAC addresses: 4
• Sticky learning: Enabled

Up to 4 MACs allowed — and sticky learning means SW2 automatically remembers the first devices it sees and locks them in. A 5th device? Traffic silently dropped and violation counter incremented. Port stays up.

