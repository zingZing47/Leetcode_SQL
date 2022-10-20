# Leetcode_SQL 


| No.           | Relevant Functions |Description|
| ------------- | -----------------| -------------|
| 176 | window: `dense_rank()`  `ifnull()`|Second Highest Salary|
| \177 | window: `dense_rank()` or `ifnull()`+`limit()` |UDFUNCTION:Nth Highest Salary|
| 180 | NO LAG() LEAD()in mySQL |Consecutive Numbers|
| 181 | self join |Employees Earning More Than Their Managers|
| 182 | Group by + having |Duplicate Emails|
| 183 | left join |Customers Who Never Order|
| 184 | window: `rank()` |Department Highest Salary|
| 185 | window: `dense_rank()` |Department Top Three Salaries|
| 262 | `BETWEEN()` |Trips and Users|
| 511 | window: `dense_rank()`  |Game Play Analysis: find first_login date|
| 550 | `AVG()`,`DATEDIFF()`,`MIN()`  |Game Play Analysis IV|
| \608 | `MOD()`, `CASE WHEN`  |Exchange Seats|
| 626 | `IS NULL`, `NOT IN`  |GTree Node| 
| \1077 | Union() or CTE: `with recursive` |Project Employees III: find the most experiecned employees|
| \1158 | `On vs Where` |Market Analysis I| 
| 1270 | window: `rank()`  |All People Report to the Given Manager|
| 1285 | window: `row_number()`  |Find the Start and End Number of Continuous Ranges|
| 1308 | window: `sum()`  |Running Total for Different Genders|
| 1369 | window: `count()+ rank()`  |Get the Second Most Recent Activity|
| \1407 | `IFNULL()`  |Top Travellers: Repeat names(don't group by)|
| 1412 | `rank()`*2: decending / ascending  |Find the Quiet Students in All Exams|
| 1532 | window: `rank()`  |The Most Recent Three Orders|
| 1549 |  `max()`  |The Most Recent Orders for Each Product: keep the duplicates|
| 1596 | window: `rank()`  |The Most Frequently Ordered Products for Each Customer|
|\1613 | CTE: `with recursive`  |Find the Missing IDs|
| 1709 | window: `LEAD()`  |Biggest Window Between Visits|
| \1767 | CTE: `with recursive`   |Find the Subtasks That Did Not Execute|
| 1949 | `Union` + `Join` |Strong Friendship|
| 1951 | window: `rank()`  |All the Pairs With the Maximum Number of Common Followers|
| 1972 | window: `dense_rank()`+ `Union` |First and Last Call On the Same Day|


262. Trips and Users


## Aggregation Functions:
sum()

avg()

mean()

max() / min()

count()


## Calculation Symbols:
’*‘ multiply

/ divid

% remainder

abs() absolute

stddev() Standard deviation

cbrt() cubed root


## Date:
date_sub('2022-8-20', INTERVAL 3 day), to create new date

date_add'2022-8-20', INTERVAL 3 day), to create new date

date_format(day,"%Y-%m-%d"), to extract only date from column 'day'

age(col1, col2), calculate the gap year between two columns, col1(later) > col2

datediff('2022-8-20','2022-8-19'), calculate the days diff between two columns, col1(later) > col2



## Operations:
coalesce() return the 1st not null value

round()

cast('2022-8-20' as DATE)  transfrom datatype

group_concat(col [ORDER BY col SEPARATOR ',']) Concatenate a column according to specific conditions
