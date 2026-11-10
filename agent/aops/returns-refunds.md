---
name: Returns & refunds
when: The customer wants to return a book or get a refund, including a book that arrived damaged.
enabled: true
force_category: returns_refunds
created_by: Patrick Phrayme
updated_by: Patrick Phrayme
updated_at: '2026-11-10T02:47:41+00:00'
---

1. If the book arrived damaged, look up the damaged-item policy with @search_policies and share it.
2. Get the order ID and the email on the account, if you don't have them yet.
3. Look up the order with @get_order_status. If it isn't eligible for return (not delivered yet, or past the 30-day window), explain why and stop.
4. If the order has more than one book, ask which one.
5. File the return with @initiate_return. Don't ask for a reason -- pass along whatever they said, or "No reason given." Share the return ID and the refund amount.
6. If the book arrived damaged, tell them they don't need to send it back. Otherwise, offer a prepaid label: unless they say no, create it with @generate_return_label and explain that the refund is issued once the book arrives back.
