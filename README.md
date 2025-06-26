Task 3: Writing Basic SELECT Queries

 Objective :
To practice writing SQL queries that extract and filter data from a table using `SELECT`, `WHERE`, `ORDER BY`, `LIMIT`, and other related clauses.


1. Created a table named `Employees` with relevant fields.
2. Inserted data using different combinations of column values.
3. Updated some records to assign bonus values.
4. Wrote various `SELECT` queries to:
   - Fetch all records
   - Fetch specific columns
   - Apply filters using `WHERE`, `AND`, `OR`
   - Use `LIKE` for pattern matching
   - Filter within a range using `BETWEEN`
   - Sort data using `ORDER BY`
   - Limit number of rows using `LIMIT`
   - Remove duplicates with `DISTINCT`
   - Use `IN` for filtering multiple values

 Table Data:
| emp_id | name   | age  | department | salary | bonus |
|--------|--------|------|------------|--------|-------|
| 1      | Anu    | 30   | HR         | 50000  | 5000  |
| 2      | Praju  | 28   | General    | 45000  | NULL  |
| 3      | Poorvi | NULL | IT         | 60000  | 2000  |

SELECT name, age → Returns names and ages of all employees
WHERE department = 'HR' → Returns Anu’s record
LIKE '%an%' → Matches Anu
WHERE department = 'HR' → Returns Praju and poovi’s record
LIKE '%p%' → Matches Praju and poovi
BETWEEN 25 AND 40 → Matches Anu and Praju
ORDER BY salary DESC → Returns Poorvi, Anu, Praju (highest to lowest)
LIMIT 5 → Returns all rows since we have only 3
Aliased Columns → name AS Employee\_Name, salary AS Monthly\_Salary
DISTINCT department → HR, General, IT
IN ('HR', 'Sales') → Returns Anu only


 Interview Questions and Answers

1. What does SELECT * do?
   Retrieves all columns from a table.

2. How do you filter rows?
   Using the WHERE clause.

3. What is LIKE '%value%'?
   Filters rows where the column contains a substring.

4. What is BETWEEN used for?
   To filter values within a given range.

5. How do you limit output rows?
   Using the LIMIT clause.

6. Difference between = and IN?
   = compares a single value, IN checks against multiple values.

7. How to sort in descending order?
   Using ORDER BY column DESC.

8. What is aliasing?
   Temporarily renaming a column using AS.

9. Explain DISTINCT.
   Removes duplicate entries in the output.

10. What is the default sort order?
    Ascending (ASC) order.


