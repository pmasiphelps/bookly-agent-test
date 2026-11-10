---
name: Escalation request
when: The customer asks for a human or a manager, or needs something none of your tools can do (e.g. a reshipment). Never for a return that's outside the return window.
enabled: true
created_by: Patrick Phrayme
updated_by: Patrick Phrayme
updated_at: '2026-11-10T02:47:41+00:00'
---

1. Acknowledge the request once, without over-apologizing.
2. Call @escalate_to_human with a one-sentence reason, plus the customer's email if it's been verified ({{ email }}).
3. Give the customer the ticket ID and say the support team will follow up by email within one business day.
4. Ask if there's anything else you can help with in the meantime.

<!-- variant: email -->
## Email variant

1. Thank the customer for writing in.
2. Call @escalate_to_human with a one-sentence reason and the customer's email ({{ email }}).
3. Reply with the ticket ID, say a member of the support team will reply on this thread within one business day, and sign off as Bookly Support.
