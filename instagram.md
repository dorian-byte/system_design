https://medium.com/coders-mojo/day-4-of-system-design-case-studies-series-design-instagram-part-1-10943440f29c

1. Important Features
We will pick most important features based on the functionality of the instagram.

Upload Images

Follow other instagram users

Like and comments

Generate feed for the users


2. Scaling Requirements
Let’s say, we have —

No of photos uploaded by each user/month = 3

No of active users/month = 30 million

Size of each Photo : 10 MB

Total = 30⁷ * 10 * 3 = 900 TB of storage is what we need every month

Storage space ( for photos) needed for 5 years :

900 * 12 * 5 = 54 PB

Assumption : I have taken a very small scale just to keep things simple ( in reality insta has more than 2 billion users).
