## 1. Current system date and time (DATETIME format)
```sql
SELECT GETDATE();
```
## 2. Extracting year, month, and day from current date
```sql
SELECT YEAR(GETDATE()) AS Year,
       MONTH(GETDATE()) AS Month,
       DAY(GETDATE()) AS Day;
```
## 3. DATEADD function is used to add or subtract a specified time interval (such as days, months, or years) to or from a date.
### Syntax: DATEADD(datepart, number, date)
### - datepart (year,month,day)
### - number (The value to add (positive) or subtract (negative))
### - date (The base date )
### EXAMPLE:
```sql
-- 7 days into the future
SELECT DATEADD(DAY, 7, GETDATE()) AS DateIn7Days;
-- 1 month into the past
SELECT DATEADD(MONTH, -1, GETDATE()) AS OneMonthAgo;
```

