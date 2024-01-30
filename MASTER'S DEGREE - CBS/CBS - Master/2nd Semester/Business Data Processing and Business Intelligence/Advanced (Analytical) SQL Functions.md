For simpler see [[SQL Queries]]. 

Analytical functions are powerful tool to build powerful reports very fast

### General Syntax of Advanced SQL Functions
The syntax can seem complicated
- A general syntax:
```SQL
AnalyticalFuncName([arguments]) 
OVER ( 
[PARTITION BY partition_expression,…] 
[ORDER BY sort_expression, … [ASC|DESC]]) 
```

- Examples:
	- Find Top 5 Stores by Sale
	- Find top Nth product with respect to sale in particular region
	- Compare Total Sale Per month with immediate previous month

## Analytical Functions
- RANK() => Assign rank to a row based on column
- FIRST_VALUE => Find first value within a group or dataset
- NTH_VALUE => Find nth value within a group or dataset
- LAG() => Display values after the occurance of current row
- LEAD() => Display values before the occurance of current row