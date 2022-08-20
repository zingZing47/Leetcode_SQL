# Leetcode_SQL

| No.           | Relevant Functions |Description|
| ------------- | -----------------| -------------|
| 177 | window: `dense_rank()` or `ifnull()`+`limit()` |UDFUNCTION:Nth Highest Salary|
| 511 | window: `dense_rank()`  |Game Play Analysis: find first_login date|
| 1077 | window: `rank()`  |Project Employees III: find the most experiecned employees|
| 1285 | window: `row_number()`  |Find the Start and End Number of Continuous Ranges|
| 1308 | window: `sum()`  |Running Total for Different Genders|
| 1407 | `IFNULL()`  |Top Travellers: Repeat names(don't group by)|
| 1549 |  `max()`  |The Most Recent Orders for Each Product: keep the duplicates|
| 1596 | window: `rank()`  |The Most Frequently Ordered Products for Each Customer|
| 1709 | window: `LEAD()`  |Biggest Window Between Visits|
| 1951 | window: `rank()`  |All the Pairs With the Maximum Number of Common Followers|

# QUICK TAKAWAYS:
## Aggregation Functions:
sum()
avg()
mean()
max() / min()
count()

## Calculation Symbols:
* multiply
/ divid
% remainder
abs() absolute
stddev() Standard deviation
cbrt() cubed root

## Date:
date_sub('2022-8-20', INTERVAL 3 day), to create new date
date_part('quarter', col_name), to select desired date type from exisiting columns ( 'year'/'month'/'day')
age(col1, col2), calculate the gap year between two columns, col1(later) > col2
datediff('2022-8-20','2022-8-19'), calculate the days diff between two columns, col1(later) > col2

## Operations:
coalesce() return the 1st not null value
round()
cast('2022-8-20' as DATE)  transfrom datatype
group_concat(col [ORDER BY col SEPARATOR ',']) Concatenate a column according to specific conditions
