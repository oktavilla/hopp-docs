Timestamps work like this:

```
If published today:
  "today 10:00"
Else if published yesterday:
  "yesterday 10:00"
Else if published within 6 days:
  "tue 10:00"
Else if NOT published current year:
  "23 mar 2020"
Else if published within 89 days:
  "23 mar 10:00"
Else:
  "23 mar 2020"
```
