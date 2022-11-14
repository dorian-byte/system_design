Details see: https://medium.com/coders-mojo/day-5-of-system-design-case-studies-series-design-messenger-app-7b73c589f4a

Features:
1. one to one message.
2. Group messaging.
3. send media.
4. Notification push.
5. User status.

Scaling requirements:

- Daily active users ( DAU) : 200 million

- Messages per user ( within a day) : 20

- Total messages/day : 4 Billion messages

- Storage Estimation —

- Message size : 80 bytes

- Total Storage per day : 4 billion messages * 80 bytes = 320 GB/day

- For next 3 years, 320 GB * 3 * 365 = 350 TB
