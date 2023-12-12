## Dates

### Functions

1. To display the current date:
```
SELECT CURRENT_DATE;
```

2. Find the date after some days fom today
```
SELECT ADDDATE(CURRENT_DATE, INTERVAL 45 DAY);
```

3. Find the number of days between two dates
```
SELECT DATEDIFF(CURRENT_DATE, '2023-01-01');
```
for not return negative dates for this function we can use ABS as:
```
SELECT ABS(ADDDATE(CURRENT_DATE, '2023-01-01'));
```
