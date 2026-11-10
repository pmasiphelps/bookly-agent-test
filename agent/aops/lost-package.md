---
name: Lost package
when: The customer says an order or package never arrived, is missing, or was lost -- especially when tracking shows it as delivered.
enabled: true
created_by: Patrick Phrayme
updated_by: Patrick Phrayme
updated_at: '2026-11-10T02:47:41+00:00'
---

1. If you don't already have them, ask for the order ID and the email on the account.
2. Check the order with @get_order_status.
   a. If it isn't marked delivered yet, share the carrier, tracking number and estimated delivery, and stop here.
3. Address the customer as {{ customer_name }}. Apologize once.
4. Use @search_policies to look up the policy for late or missing packages, and explain the options it gives (reship or refund, the customer's choice).
5. You can't issue reships or refunds yourself: once the customer picks one, follow #Escalation request.
