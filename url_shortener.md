Important Features
Convert Long URL to Tiny URL

Convert Tiny URL into Long URL

Scaling Requirements — Capacity Estimation
Let’s say —

About ~80 Million URL’s are generated everyday.

Write operations per second —

80Million/24/3600 = 930 write operations per second

Let’ assume, read to write ratio is 8:1, then read operations per second —

930 * 8 = 7440 read operations per second

Average URL length is 90bytes

Storage Requirement —

80 Million * 90 = 7GB /day

No of records after 5 years —

80Million * 365 * 5 = 146 Billion

For next 5 years, the storage requirements would be —

90Bytes * 5 * 146 Billion = 65.7 TB

Data Model — ER requirements
User

User_id: Int

Username: String

Email : String

Date_of_creation: Datetime

Functionality —

Users should be able to shorten the url.

Users should be able to get the original url from the shortened url.

— — — — — — — — — — — — — — — — — — — — — — — — — — — — —

URL table

short_url_id : Int

long_url_id : Int

short_url_text: String

Long_url_text: String

Functionality —

Store/compute the shorten url and long url.
