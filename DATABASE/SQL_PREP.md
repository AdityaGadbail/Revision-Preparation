# SQL Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of SQL interview questions — from fundamentals to joins, aggregation, indexing, transactions, and window functions — with clear answers and code examples where they help. Built to be your one-stop revision resource the night before an interview or test.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#most-asked-tricky-questions)
  - [What is the difference between `WHERE` and `HAVING`?](#what-is-the-difference-between-where-and-having)
  - [What is the difference between `INNER JOIN` and `LEFT JOIN`?](#what-is-the-difference-between-inner-join-and-left-join)
  - [What is the difference between `DELETE`, `TRUNCATE`, and `DROP`?](#what-is-the-difference-between-delete-truncate-and-drop)
  - [What is the difference between a primary key and a unique key?](#what-is-the-difference-between-a-primary-key-and-a-unique-key)
  - [What is a JOIN, and what are the main types?](#what-is-a-join-and-what-are-the-main-types)
  - [What is the difference between `UNION` and `UNION ALL`?](#what-is-the-difference-between-union-and-union-all)
  - [What is a subquery, and what's the difference between a correlated and non-correlated subquery?](#what-is-a-subquery-and-whats-the-difference-between-a-correlated-and-non-correlated-subquery)
  - [What is normalization, and what problem does it solve?](#what-is-normalization-and-what-problem-does-it-solve)
  - [What is an index, and how does it improve query performance?](#what-is-an-index-and-how-does-it-improve-query-performance)
  - [What is a transaction, and what does ACID stand for?](#what-is-a-transaction-and-what-does-acid-stand-for)
  - [What is the difference between `GROUP BY` and `ORDER BY`?](#what-is-the-difference-between-group-by-and-order-by)
  - [What is a self-join, and when would you use one?](#what-is-a-self-join-and-when-would-you-use-one)
  - [What is the difference between a clustered index and a non-clustered index?](#what-is-the-difference-between-a-clustered-index-and-a-non-clustered-index)
  - [What is a foreign key, and what is referential integrity?](#what-is-a-foreign-key-and-what-is-referential-integrity)
  - [What is the difference between `NULL` and an empty string?](#what-is-the-difference-between-null-and-an-empty-string)
  - [How do you find the second-highest value in a column using SQL?](#how-do-you-find-the-second-highest-value-in-a-column-using-sql)
- [SQL Basics](#sql-basics)
  - [What is SQL, and what is it used for?](#what-is-sql-and-what-is-it-used-for)
  - [What are the main categories of SQL commands?](#what-are-the-main-categories-of-sql-commands)
  - [What is the basic syntax of a `SELECT` statement?](#what-is-the-basic-syntax-of-a-select-statement)
  - [What is the difference between `CHAR` and `VARCHAR` data types?](#what-is-the-difference-between-char-and-varchar-data-types)
  - [What is the difference between `DISTINCT` and `GROUP BY` for removing duplicates?](#what-is-the-difference-between-distinct-and-group-by-for-removing-duplicates)
  - [What is a `LIKE` clause used for, and what do `%` and `_` wildcards mean?](#what-is-a-like-clause-used-for-and-what-do-and-wildcards-mean)
  - [What is the difference between `IN` and `EXISTS`?](#what-is-the-difference-between-in-and-exists)
  - [What is the difference between `BETWEEN` and using `>=`/`<=`?](#what-is-the-difference-between-between-and-using)
  - [What is an alias in SQL, and how do you create one?](#what-is-an-alias-in-sql-and-how-do-you-create-one)
  - [What is the difference between `COUNT(*)`, `COUNT(column)`, and `COUNT(DISTINCT column)`?](#what-is-the-difference-between-count-countcolumn-and-countdistinct-column)
  - [What is the difference between `IS NULL` and `= NULL`?](#what-is-the-difference-between-is-null-and-null)
  - [What is the logical order of execution of clauses in a SQL query?](#what-is-the-logical-order-of-execution-of-clauses-in-a-sql-query)
- [Joins](#joins)
  - [What does an `INNER JOIN` return?](#what-does-an-inner-join-return)
  - [What does a `LEFT JOIN` return?](#what-does-a-left-join-return)
  - [What does a `RIGHT JOIN` return, and how does it relate to `LEFT JOIN`?](#what-does-a-right-join-return-and-how-does-it-relate-to-left-join)
  - [What does a `FULL OUTER JOIN` return?](#what-does-a-full-outer-join-return)
  - [What is a `CROSS JOIN`, and when would you use one?](#what-is-a-cross-join-and-when-would-you-use-one)
  - [What is a self-join, and can you give an example?](#what-is-a-self-join-and-can-you-give-an-example)
  - [What is the difference between explicit `JOIN` syntax and the older implicit comma-based join syntax?](#what-is-the-difference-between-explicit-join-syntax-and-the-older-implicit-comma-based-join-syntax)
  - [How would you find rows that exist in one table but not in another?](#how-would-you-find-rows-that-exist-in-one-table-but-not-in-another)
  - [Can you join more than two tables in a single query?](#can-you-join-more-than-two-tables-in-a-single-query)
  - [What is a common performance pitfall with joins on large tables, and how do you mitigate it?](#what-is-a-common-performance-pitfall-with-joins-on-large-tables-and-how-do-you-mitigate-it)
- [Aggregation & Grouping](#aggregation-grouping)
  - [What are aggregate functions? Name some common ones.](#what-are-aggregate-functions-name-some-common-ones)
  - [What does `GROUP BY` do, and what's a common rule about columns in the `SELECT` list?](#what-does-group-by-do-and-whats-a-common-rule-about-columns-in-the-select-list)
  - [How do you filter groups after aggregation, and why can't you use `WHERE` for that?](#how-do-you-filter-groups-after-aggregation-and-why-cant-you-use-where-for-that)
  - [What is the difference between `GROUP BY` with multiple columns vs. a single column?](#what-is-the-difference-between-group-by-with-multiple-columns-vs-a-single-column)
  - [How do `NULL` values behave in `GROUP BY` and aggregate functions?](#how-do-null-values-behave-in-group-by-and-aggregate-functions)
  - [What is `ROLLUP`, and what does it add to a `GROUP BY` query?](#what-is-rollup-and-what-does-it-add-to-a-group-by-query)
  - [What is the difference between `GROUP BY` and using a window function for aggregation?](#what-is-the-difference-between-group-by-and-using-a-window-function-for-aggregation)
  - [How would you find duplicate rows in a table based on a specific column?](#how-would-you-find-duplicate-rows-in-a-table-based-on-a-specific-column)
  - [What is the difference between `SUM()` and `COUNT()` when a column contains `NULL` values?](#what-is-the-difference-between-sum-and-count-when-a-column-contains-null-values)
  - [How would you calculate a percentage of a total within each group using aggregation?](#how-would-you-calculate-a-percentage-of-a-total-within-each-group-using-aggregation)
- [Subqueries & CTEs](#subqueries-ctes)
  - [What is a subquery, and where can it be used?](#what-is-a-subquery-and-where-can-it-be-used)
  - [What is the difference between a correlated and non-correlated subquery?](#what-is-the-difference-between-a-correlated-and-non-correlated-subquery)
  - [What is a Common Table Expression (CTE), and what does the `WITH` clause do?](#what-is-a-common-table-expression-cte-and-what-does-the-with-clause-do)
  - [What is a recursive CTE, and what problem does it solve?](#what-is-a-recursive-cte-and-what-problem-does-it-solve)
  - [What is the difference between a CTE and a subquery in the `FROM` clause?](#what-is-the-difference-between-a-cte-and-a-subquery-in-the-from-clause)
  - [What is the difference between a scalar subquery and a subquery used with `IN`?](#what-is-the-difference-between-a-scalar-subquery-and-a-subquery-used-with-in)
  - [Can a subquery return multiple columns, and where would that be valid?](#can-a-subquery-return-multiple-columns-and-where-would-that-be-valid)
  - [What is a common performance concern with correlated subqueries, and how might you rewrite one to avoid it?](#what-is-a-common-performance-concern-with-correlated-subqueries-and-how-might-you-rewrite-one-to-avoid-it)
  - [What is the difference between `EXISTS` and `IN` in terms of handling `NULL` values?](#what-is-the-difference-between-exists-and-in-in-terms-of-handling-null-values)
  - [How would you use a CTE to simplify a query that otherwise needs a subquery repeated multiple times?](#how-would-you-use-a-cte-to-simplify-a-query-that-otherwise-needs-a-subquery-repeated-multiple-times)
- [Indexes & Query Optimization](#indexes-query-optimization)
  - [What is an index, and what data structure do most databases use for one?](#what-is-an-index-and-what-data-structure-do-most-databases-use-for-one)
  - [What is the difference between a clustered and non-clustered index?](#what-is-the-difference-between-a-clustered-and-non-clustered-index)
  - [What is a composite (multi-column) index, and does column order matter?](#what-is-a-composite-multi-column-index-and-does-column-order-matter)
  - [What are the trade-offs of adding more indexes to a table?](#what-are-the-trade-offs-of-adding-more-indexes-to-a-table)
  - [What is the `EXPLAIN` command used for?](#what-is-the-explain-command-used-for)
  - [What is a full table scan, and why is it usually something to avoid on large tables?](#what-is-a-full-table-scan-and-why-is-it-usually-something-to-avoid-on-large-tables)
  - [What is index selectivity, and why does it matter?](#what-is-index-selectivity-and-why-does-it-matter)
  - [What is a covering index?](#what-is-a-covering-index)
  - [How can using a function on an indexed column in a `WHERE` clause hurt performance?](#how-can-using-a-function-on-an-indexed-column-in-a-where-clause-hurt-performance)
  - [What is query plan caching, and why does it matter for repeated queries?](#what-is-query-plan-caching-and-why-does-it-matter-for-repeated-queries)
- [Normalization & Database Design](#normalization-database-design)
  - [What is database normalization, and what problem does it solve?](#what-is-database-normalization-and-what-problem-does-it-solve)
  - [What is First Normal Form (1NF)?](#what-is-first-normal-form-1nf)
  - [What is Second Normal Form (2NF)?](#what-is-second-normal-form-2nf)
  - [What is Third Normal Form (3NF)?](#what-is-third-normal-form-3nf)
  - [What are insertion, update, and deletion anomalies, and how does normalization prevent them?](#what-are-insertion-update-and-deletion-anomalies-and-how-does-normalization-prevent-them)
  - [What is denormalization, and why might you intentionally denormalize a database?](#what-is-denormalization-and-why-might-you-intentionally-denormalize-a-database)
  - [What is a composite key?](#what-is-a-composite-key)
  - [What is a surrogate key, and how does it differ from a natural key?](#what-is-a-surrogate-key-and-how-does-it-differ-from-a-natural-key)
  - [What is an Entity-Relationship (ER) diagram, and why is it useful in database design?](#what-is-an-entity-relationship-er-diagram-and-why-is-it-useful-in-database-design)
  - [When might you choose to design a table with a many-to-many relationship, and how do you implement it in SQL?](#when-might-you-choose-to-design-a-table-with-a-many-to-many-relationship-and-how-do-you-implement-it-in-sql)
- [Constraints & Keys](#constraints-keys)
  - [What is a `PRIMARY KEY` constraint, and what does it enforce?](#what-is-a-primary-key-constraint-and-what-does-it-enforce)
  - [What is a `FOREIGN KEY` constraint, and what does it enforce?](#what-is-a-foreign-key-constraint-and-what-does-it-enforce)
  - [What is a `UNIQUE` constraint, and how does it differ from a `PRIMARY KEY`?](#what-is-a-unique-constraint-and-how-does-it-differ-from-a-primary-key)
  - [What is a `CHECK` constraint?](#what-is-a-check-constraint)
  - [What is a `NOT NULL` constraint?](#what-is-a-not-null-constraint)
  - [What does `ON DELETE CASCADE` do on a foreign key?](#what-does-on-delete-cascade-do-on-a-foreign-key)
  - [What is the difference between `ON DELETE CASCADE`, `ON DELETE SET NULL`, and `ON DELETE RESTRICT`?](#what-is-the-difference-between-on-delete-cascade-on-delete-set-null-and-on-delete-restrict)
  - [What is a `DEFAULT` constraint?](#what-is-a-default-constraint)
- [Transactions & ACID](#transactions-acid)
  - [What is a database transaction?](#what-is-a-database-transaction)
  - [What does ACID stand for, and briefly explain each property.](#what-does-acid-stand-for-and-briefly-explain-each-property)
  - [What is the difference between `COMMIT` and `ROLLBACK`?](#what-is-the-difference-between-commit-and-rollback)
  - [What is a `SAVEPOINT`, and why would you use one?](#what-is-a-savepoint-and-why-would-you-use-one)
  - [What are the standard transaction isolation levels, from least to most strict?](#what-are-the-standard-transaction-isolation-levels-from-least-to-most-strict)
  - [What is a dirty read?](#what-is-a-dirty-read)
  - [What is a non-repeatable read?](#what-is-a-non-repeatable-read)
  - [What is a phantom read?](#what-is-a-phantom-read)
  - [What is a deadlock, and how do databases typically handle one?](#what-is-a-deadlock-and-how-do-databases-typically-handle-one)
  - [What is optimistic locking, and how does it differ from pessimistic locking?](#what-is-optimistic-locking-and-how-does-it-differ-from-pessimistic-locking)
- [Window Functions](#window-functions)
  - [What is a window function, and how does it differ from a regular aggregate function used with `GROUP BY`?](#what-is-a-window-function-and-how-does-it-differ-from-a-regular-aggregate-function-used-with-group-by)
  - [What does the `OVER()` clause do?](#what-does-the-over-clause-do)
  - [What is the difference between `RANK()`, `DENSE_RANK()`, and `ROW_NUMBER()`?](#what-is-the-difference-between-rank-denserank-and-rownumber)
  - [What does `PARTITION BY` do within a window function, and how does it differ from `GROUP BY`?](#what-does-partition-by-do-within-a-window-function-and-how-does-it-differ-from-group-by)
  - [What are the `LAG()` and `LEAD()` functions used for?](#what-are-the-lag-and-lead-functions-used-for)
  - [What is the difference between `NTILE(n)` and `RANK()`?](#what-is-the-difference-between-ntilen-and-rank)
  - [How would you calculate a running total using a window function?](#how-would-you-calculate-a-running-total-using-a-window-function)
  - [What is a window frame, and how do `ROWS BETWEEN` and `RANGE BETWEEN` differ?](#what-is-a-window-frame-and-how-do-rows-between-and-range-between-differ)
  - [Can you use a window function's result directly in a `WHERE` clause?](#can-you-use-a-window-functions-result-directly-in-a-where-clause)
  - [How would you find, for each department, the employee with the highest salary using a window function?](#how-would-you-find-for-each-department-the-employee-with-the-highest-salary-using-a-window-function)
- [Views, Stored Procedures & Triggers](#views-stored-procedures-triggers)
  - [What is a view, and what are its main benefits?](#what-is-a-view-and-what-are-its-main-benefits)
  - [What is the difference between a regular view and a materialized view?](#what-is-the-difference-between-a-regular-view-and-a-materialized-view)
  - [What is a stored procedure, and what are its advantages?](#what-is-a-stored-procedure-and-what-are-its-advantages)
  - [What is the difference between a stored procedure and a function in SQL?](#what-is-the-difference-between-a-stored-procedure-and-a-function-in-sql)
  - [What is a trigger, and what are common events that can fire one?](#what-is-a-trigger-and-what-are-common-events-that-can-fire-one)
  - [What is a potential downside of relying heavily on triggers?](#what-is-a-potential-downside-of-relying-heavily-on-triggers)
  - [Can a view be updated, and what conditions typically need to be met?](#can-a-view-be-updated-and-what-conditions-typically-need-to-be-met)
  - [What is the difference between `BEFORE` and `AFTER` triggers?](#what-is-the-difference-between-before-and-after-triggers)
- [Common Coding Challenges](#common-coding-challenges)
  - [Write a query to find the second-highest salary in a table.](#write-a-query-to-find-the-second-highest-salary-in-a-table)
  - [Write a query to find duplicate email addresses in a users table.](#write-a-query-to-find-duplicate-email-addresses-in-a-users-table)
  - [Write a query to find employees who earn more than their manager.](#write-a-query-to-find-employees-who-earn-more-than-their-manager)
  - [Write a query to delete duplicate rows, keeping only one copy of each.](#write-a-query-to-delete-duplicate-rows-keeping-only-one-copy-of-each)
  - [Write a query to find the Nth highest salary using a window function.](#write-a-query-to-find-the-nth-highest-salary-using-a-window-function)
  - [Write a query to calculate month-over-month percentage growth in revenue.](#write-a-query-to-calculate-month-over-month-percentage-growth-in-revenue)
  - [Write a query using a recursive CTE to find all subordinates under a given manager.](#write-a-query-using-a-recursive-cte-to-find-all-subordinates-under-a-given-manager)
  - [Write a query to pivot rows into columns, e.g. showing total sales per quarter as separate columns.](#write-a-query-to-pivot-rows-into-columns-eg-showing-total-sales-per-quarter-as-separate-columns)
  - [Write a query to find customers who have never placed an order.](#write-a-query-to-find-customers-who-have-never-placed-an-order)
  - [Write a query to find the top 3 products by total revenue.](#write-a-query-to-find-the-top-3-products-by-total-revenue)
- [Behavioral / Scenario-Based Questions](#behavioral-scenario-based-questions)
  - [How would you approach optimizing a slow-running query in production?](#how-would-you-approach-optimizing-a-slow-running-query-in-production)
  - [How would you design a database schema for an e-commerce platform's orders and products?](#how-would-you-design-a-database-schema-for-an-e-commerce-platforms-orders-and-products)
  - [How would you handle a situation where two transactions are deadlocking each other in production?](#how-would-you-handle-a-situation-where-two-transactions-are-deadlocking-each-other-in-production)
  - [How would you decide between normalizing and denormalizing a particular part of a schema?](#how-would-you-decide-between-normalizing-and-denormalizing-a-particular-part-of-a-schema)
  - [How would you migrate a large production table's schema, e.g. adding a new column, with minimal downtime?](#how-would-you-migrate-a-large-production-tables-schema-eg-adding-a-new-column-with-minimal-downtime)
  - [How would you investigate data inconsistency between two related tables that should always stay in sync?](#how-would-you-investigate-data-inconsistency-between-two-related-tables-that-should-always-stay-in-sync)
  - [How would you choose between using a stored procedure and handling logic in the application code?](#how-would-you-choose-between-using-a-stored-procedure-and-handling-logic-in-the-application-code)
  - [How would you approach reviewing a teammate's SQL migration or query in a code review?](#how-would-you-approach-reviewing-a-teammates-sql-migration-or-query-in-a-code-review)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="most-asked-tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every SQL interview. If you're short on time, start here.

<a id="what-is-the-difference-between-where-and-having"></a>
### Q: What is the difference between `WHERE` and `HAVING`?
**Answer:** `WHERE` filters individual rows before any grouping happens, and can't reference aggregate functions. `HAVING` filters groups after `GROUP BY` has been applied, and is specifically meant to filter based on aggregate results like `COUNT(*)` or `SUM(amount)`.

<a id="what-is-the-difference-between-inner-join-and-left-join"></a>
### Q: What is the difference between `INNER JOIN` and `LEFT JOIN`?
**Answer:** `INNER JOIN` returns only rows that have a matching row in both tables. `LEFT JOIN` returns all rows from the left table, plus matching rows from the right table where they exist, filling in `NULL` for the right table's columns when there's no match.

<a id="what-is-the-difference-between-delete-truncate-and-drop"></a>
### Q: What is the difference between `DELETE`, `TRUNCATE`, and `DROP`?
**Answer:** `DELETE` removes rows matching a condition (or all rows if no condition is given), is logged row-by-row, can be rolled back, and can fire triggers. `TRUNCATE` removes ALL rows at once, is minimally logged (faster), typically resets auto-increment counters, and generally can't be conditionally filtered. `DROP` removes the entire table structure itself, along with its data, from the database.

<a id="what-is-the-difference-between-a-primary-key-and-a-unique-key"></a>
### Q: What is the difference between a primary key and a unique key?
**Answer:** A table can have only ONE primary key, which cannot contain `NULL` values and uniquely identifies each row. A table can have MULTIPLE unique keys, which enforce uniqueness but can allow one `NULL` value in most databases, since `NULL` is considered "unknown" and not equal to another `NULL`.

<a id="what-is-a-join-and-what-are-the-main-types"></a>
### Q: What is a JOIN, and what are the main types?
**Answer:** A `JOIN` combines rows from two or more tables based on a related column. Main types: `INNER JOIN` (only matching rows), `LEFT JOIN`/`RIGHT JOIN` (all rows from one side plus matches from the other), `FULL OUTER JOIN` (all rows from both sides), and `CROSS JOIN` (every combination of rows from both tables, a Cartesian product).

<a id="what-is-the-difference-between-union-and-union-all"></a>
### Q: What is the difference between `UNION` and `UNION ALL`?
**Answer:** `UNION` combines the result sets of two queries and removes duplicate rows, which requires an extra sort/comparison step. `UNION ALL` combines them without removing duplicates, making it faster since it skips that de-duplication work — use it whenever you know there won't be duplicates or don't care about them.

<a id="what-is-a-subquery-and-whats-the-difference-between-a-correlated-and-non-correlated-subquery"></a>
### Q: What is a subquery, and what's the difference between a correlated and non-correlated subquery?
**Answer:** A subquery is a query nested inside another query. A non-correlated subquery runs independently and only once, with its result used by the outer query. A correlated subquery references a column from the outer query, so it must be logically re-evaluated for each row the outer query processes, which can be much slower on large datasets.

<a id="what-is-normalization-and-what-problem-does-it-solve"></a>
### Q: What is normalization, and what problem does it solve?
**Answer:** Normalization is the process of organizing tables and columns to minimize data redundancy and avoid update/insert/delete anomalies, typically by splitting data into multiple related tables linked by foreign keys, following a series of formal rules called normal forms (1NF, 2NF, 3NF, and beyond).

<a id="what-is-an-index-and-how-does-it-improve-query-performance"></a>
### Q: What is an index, and how does it improve query performance?
**Answer:** An index is a separate data structure (commonly a B-tree) that stores a sorted reference to column values and the rows they belong to, letting the database quickly locate matching rows without scanning the entire table — much like a book's index lets you jump straight to a page instead of reading cover to cover.

<a id="what-is-a-transaction-and-what-does-acid-stand-for"></a>
### Q: What is a transaction, and what does ACID stand for?
**Answer:** A transaction is a sequence of one or more SQL operations executed as a single logical unit of work, which either fully succeeds or fully fails. ACID stands for Atomicity (all-or-nothing), Consistency (valid state to valid state), Isolation (concurrent transactions don't interfere with each other), and Durability (once committed, changes survive even a crash).

<a id="what-is-the-difference-between-group-by-and-order-by"></a>
### Q: What is the difference between `GROUP BY` and `ORDER BY`?
**Answer:** `GROUP BY` collapses multiple rows sharing the same value(s) in specified columns into a single summary row per group, typically used alongside aggregate functions. `ORDER BY` simply controls the sort order of the final result set — it doesn't combine or reduce rows at all.

<a id="what-is-a-self-join-and-when-would-you-use-one"></a>
### Q: What is a self-join, and when would you use one?
**Answer:** A self-join joins a table to itself, treated as if it were two separate tables using table aliases to distinguish them — commonly used for hierarchical data, like an employee table referencing a manager who is also an employee, or comparing rows within the same table.

<a id="what-is-the-difference-between-a-clustered-index-and-a-non-clustered-index"></a>
### Q: What is the difference between a clustered index and a non-clustered index?
**Answer:** A clustered index determines the actual physical storage order of the table's rows on disk — a table can have only one, since data can only be physically sorted one way. A non-clustered index is a separate structure holding a sorted copy of key column values plus a pointer back to the actual row, allowing a table to have multiple non-clustered indexes.

<a id="what-is-a-foreign-key-and-what-is-referential-integrity"></a>
### Q: What is a foreign key, and what is referential integrity?
**Answer:** A foreign key is a column (or set of columns) in one table that references the primary key of another table, establishing a link between the two. Referential integrity is the guarantee that this link stays valid — you can't insert a row referencing a non-existent parent row, and, depending on configured rules, deleting or updating a referenced parent row can cascade, restrict, or set the child's reference to `NULL`.

<a id="what-is-the-difference-between-null-and-an-empty-string"></a>
### Q: What is the difference between `NULL` and an empty string?
**Answer:** `NULL` represents an unknown or missing value entirely — any arithmetic or comparison involving `NULL` (except `IS NULL`) itself returns `NULL`/unknown rather than `TRUE` or `FALSE`. An empty string (`''`) is an actual, defined value of zero length — it equals another empty string in a comparison, `NULL` does not.

<a id="how-do-you-find-the-second-highest-value-in-a-column-using-sql"></a>
### Q: How do you find the second-highest value in a column using SQL?
**Answer:** Either a subquery filtering out the maximum, or a window function like `DENSE_RANK()` ordered descending, then filtering to the second rank.

**Example:**
```sql
SELECT MAX(salary) AS second_highest
FROM employees
WHERE salary < (SELECT MAX(salary) FROM employees);
```

---

<a id="sql-basics"></a>
## SQL Basics

<a id="what-is-sql-and-what-is-it-used-for"></a>
### Q: What is SQL, and what is it used for?
**Answer:** SQL (Structured Query Language) is the standard language for creating, querying, updating, and managing data in relational database management systems (RDBMS) like PostgreSQL, MySQL, SQL Server, and Oracle.

<a id="what-are-the-main-categories-of-sql-commands"></a>
### Q: What are the main categories of SQL commands?
**Answer:** DDL (Data Definition Language: `CREATE`, `ALTER`, `DROP` — defines schema structure), DML (Data Manipulation Language: `SELECT`, `INSERT`, `UPDATE`, `DELETE` — manages actual data), DCL (Data Control Language: `GRANT`, `REVOKE` — manages permissions), and TCL (Transaction Control Language: `COMMIT`, `ROLLBACK`, `SAVEPOINT` — manages transactions).

<a id="what-is-the-basic-syntax-of-a-select-statement"></a>
### Q: What is the basic syntax of a `SELECT` statement?
**Answer:** A `SELECT` statement specifies which columns to retrieve, from which table, with optional filtering and ordering.

**Example:**
```sql
SELECT column1, column2
FROM table_name
WHERE condition
ORDER BY column1;
```

<a id="what-is-the-difference-between-char-and-varchar-data-types"></a>
### Q: What is the difference between `CHAR` and `VARCHAR` data types?
**Answer:** `CHAR(n)` is a fixed-length string type — always stores exactly `n` characters, padding shorter values with spaces, which can waste storage but has slightly predictable performance. `VARCHAR(n)` is variable-length — stores only as many characters as actually used up to the max `n`, generally more space-efficient for varying-length data.

<a id="what-is-the-difference-between-distinct-and-group-by-for-removing-duplicates"></a>
### Q: What is the difference between `DISTINCT` and `GROUP BY` for removing duplicates?
**Answer:** `DISTINCT` simply removes exact duplicate rows from the result set based on the selected columns. `GROUP BY` groups rows sharing the same values together and is typically paired with aggregate functions to compute something about each group, not just deduplicate — though `GROUP BY` alone can also produce a deduplication effect similar to `DISTINCT`.

<a id="what-is-a-like-clause-used-for-and-what-do-and-wildcards-mean"></a>
### Q: What is a `LIKE` clause used for, and what do `%` and `_` wildcards mean?
**Answer:** `LIKE` performs pattern matching on string columns. `%` matches any sequence of zero or more characters; `_` matches exactly one single character.

**Example:**
```sql
SELECT * FROM users WHERE name LIKE 'J%';   -- starts with J
SELECT * FROM users WHERE name LIKE '_ohn'; -- matches "John", "Bohn", etc.
```

<a id="what-is-the-difference-between-in-and-exists"></a>
### Q: What is the difference between `IN` and `EXISTS`?
**Answer:** `IN` checks whether a value matches any value in a given list or subquery result. `EXISTS` checks only whether a subquery returns any rows at all, without caring about their actual values — often more efficient for correlated subqueries since it can stop as soon as it finds one matching row.

<a id="what-is-the-difference-between-between-and-using"></a>
### Q: What is the difference between `BETWEEN` and using `>=`/`<=`?
**Answer:** `BETWEEN a AND b` is inclusive shorthand equivalent to `column >= a AND column <= b` — functionally identical, just more concise and often more readable for range conditions.

<a id="what-is-an-alias-in-sql-and-how-do-you-create-one"></a>
### Q: What is an alias in SQL, and how do you create one?
**Answer:** An alias gives a table or column a temporary alternate name within a query, using the `AS` keyword (often optional), improving readability or resolving naming conflicts, especially in joins.

**Example:**
```sql
SELECT u.name AS user_name, o.total AS order_total
FROM users AS u
JOIN orders AS o ON u.id = o.user_id;
```

<a id="what-is-the-difference-between-count-countcolumn-and-countdistinct-column"></a>
### Q: What is the difference between `COUNT(*)`, `COUNT(column)`, and `COUNT(DISTINCT column)`?
**Answer:** `COUNT(*)` counts ALL rows in the group, regardless of `NULL` values. `COUNT(column)` counts only rows where that specific column is not `NULL`. `COUNT(DISTINCT column)` counts only the distinct non-`NULL` values in that column.

<a id="what-is-the-difference-between-is-null-and-null"></a>
### Q: What is the difference between `IS NULL` and `= NULL`?
**Answer:** `= NULL` never evaluates to `TRUE` — since `NULL` represents an unknown value, comparing anything to it with `=` also yields unknown/`NULL`, not `TRUE` or `FALSE`. You must use the dedicated `IS NULL` (or `IS NOT NULL`) operator to correctly check for `NULL` values.

<a id="what-is-the-logical-order-of-execution-of-clauses-in-a-sql-query"></a>
### Q: What is the logical order of execution of clauses in a SQL query?
**Answer:** Roughly: `FROM` (and `JOIN`s) → `WHERE` → `GROUP BY` → `HAVING` → `SELECT` → `DISTINCT` → `ORDER BY` → `LIMIT`/`OFFSET` — which is why you can't reference a `SELECT` column alias in a `WHERE` clause (it doesn't exist yet at that stage), but you often can in `ORDER BY`.

---

<a id="joins"></a>
## Joins

<a id="what-does-an-inner-join-return"></a>
### Q: What does an `INNER JOIN` return?
**Answer:** Only the rows where the join condition matches in BOTH tables — rows with no match on either side are excluded entirely from the result.

**Example:**
```sql
SELECT o.id, c.name
FROM orders o
INNER JOIN customers c ON o.customer_id = c.id;
```

<a id="what-does-a-left-join-return"></a>
### Q: What does a `LEFT JOIN` return?
**Answer:** ALL rows from the left (first-listed) table, plus matching rows from the right table where a match exists — any right-table columns are filled with `NULL` when there's no matching row.

<a id="what-does-a-right-join-return-and-how-does-it-relate-to-left-join"></a>
### Q: What does a `RIGHT JOIN` return, and how does it relate to `LEFT JOIN`?
**Answer:** The mirror image of `LEFT JOIN` — it returns ALL rows from the right table, plus matching rows from the left table, filling `NULL` where there's no match. Any `RIGHT JOIN` can be rewritten as an equivalent `LEFT JOIN` simply by swapping the order the tables are listed in.

<a id="what-does-a-full-outer-join-return"></a>
### Q: What does a `FULL OUTER JOIN` return?
**Answer:** ALL rows from BOTH tables — matched rows are combined normally, while unmatched rows from either side appear with `NULL`s filling in for the columns of whichever table didn't have a match.

<a id="what-is-a-cross-join-and-when-would-you-use-one"></a>
### Q: What is a `CROSS JOIN`, and when would you use one?
**Answer:** A `CROSS JOIN` produces the Cartesian product of two tables — every row from the first table paired with every row from the second, with no join condition at all. Genuinely useful cases are rare, like generating all possible combinations of two small sets (sizes × colors for product variants), and it can produce enormous result sets on large tables if used accidentally.

<a id="what-is-a-self-join-and-can-you-give-an-example"></a>
### Q: What is a self-join, and can you give an example?
**Answer:** A join where a table is joined to itself, using two different aliases to treat it as if it were two separate tables — commonly used for hierarchical relationships.

**Example:**
```sql
SELECT e.name AS employee, m.name AS manager
FROM employees e
LEFT JOIN employees m ON e.manager_id = m.id;
```

<a id="what-is-the-difference-between-explicit-join-syntax-and-the-older-implicit-comma-based-join-syntax"></a>
### Q: What is the difference between explicit `JOIN` syntax and the older implicit comma-based join syntax?
**Answer:** Explicit syntax (`FROM a JOIN b ON a.id = b.a_id`) clearly separates the join condition from filtering conditions in `WHERE`, and makes outer joins possible. The older implicit syntax (`FROM a, b WHERE a.id = b.a_id`) mixes join conditions into `WHERE`, is easier to accidentally turn into an unintended cross join, and cannot express outer joins at all in standard SQL — explicit `JOIN` syntax is universally recommended today.

<a id="how-would-you-find-rows-that-exist-in-one-table-but-not-in-another"></a>
### Q: How would you find rows that exist in one table but not in another?
**Answer:** Use a `LEFT JOIN` combined with a `WHERE ... IS NULL` check on the right table's key — rows with no match will have `NULL` there — or equivalently use `NOT EXISTS` with a correlated subquery, which is often more efficient.

**Example:**
```sql
SELECT c.*
FROM customers c
LEFT JOIN orders o ON c.id = o.customer_id
WHERE o.id IS NULL;
```

<a id="can-you-join-more-than-two-tables-in-a-single-query"></a>
### Q: Can you join more than two tables in a single query?
**Answer:** Yes — simply chain additional `JOIN` clauses, one after another, each specifying its own `ON` condition; there's no limit, beyond practical performance/readability, to how many tables you can join in one query.

<a id="what-is-a-common-performance-pitfall-with-joins-on-large-tables-and-how-do-you-mitigate-it"></a>
### Q: What is a common performance pitfall with joins on large tables, and how do you mitigate it?
**Answer:** Joining on columns without an index forces the database to compare every row of one table against every row of the other, which can be extremely slow on large tables. Mitigate this by ensuring the columns used in join conditions, especially foreign keys, are properly indexed.

---

<a id="aggregation-grouping"></a>
## Aggregation & Grouping

<a id="what-are-aggregate-functions-name-some-common-ones"></a>
### Q: What are aggregate functions? Name some common ones.
**Answer:** Functions that compute a single summary value from multiple rows. Common ones: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`.

<a id="what-does-group-by-do-and-whats-a-common-rule-about-columns-in-the-select-list"></a>
### Q: What does `GROUP BY` do, and what's a common rule about columns in the `SELECT` list?
**Answer:** `GROUP BY` collapses rows sharing the same value(s) in the specified column(s) into one row per group. Any non-aggregated column in the `SELECT` list generally must also appear in the `GROUP BY` clause — otherwise it's ambiguous which of the group's multiple values for that column should be shown.

<a id="how-do-you-filter-groups-after-aggregation-and-why-cant-you-use-where-for-that"></a>
### Q: How do you filter groups after aggregation, and why can't you use `WHERE` for that?
**Answer:** Use `HAVING`, which runs after grouping/aggregation — `WHERE` runs before grouping and has no way to reference an aggregate result like `SUM(amount)` since those values don't exist yet at that stage.

**Example:**
```sql
SELECT customer_id, SUM(amount) AS total
FROM orders
GROUP BY customer_id
HAVING SUM(amount) > 1000;
```

<a id="what-is-the-difference-between-group-by-with-multiple-columns-vs-a-single-column"></a>
### Q: What is the difference between `GROUP BY` with multiple columns vs. a single column?
**Answer:** Grouping by multiple columns creates one group for each unique combination of values across all the listed columns, rather than grouping by just one column's values alone — useful for more granular summaries, like total sales per customer per month, not just per customer overall.

<a id="how-do-null-values-behave-in-group-by-and-aggregate-functions"></a>
### Q: How do `NULL` values behave in `GROUP BY` and aggregate functions?
**Answer:** `GROUP BY` treats all `NULL` values in a grouping column as belonging to the same single group. Aggregate functions like `SUM()`, `AVG()`, and `COUNT(column)` simply ignore `NULL` values in their calculations — they don't count as zero — though `COUNT(*)` counts every row regardless.

<a id="what-is-rollup-and-what-does-it-add-to-a-group-by-query"></a>
### Q: What is `ROLLUP`, and what does it add to a `GROUP BY` query?
**Answer:** `ROLLUP` extends `GROUP BY` to also produce subtotal rows at each level of grouping, plus a grand total row — useful for hierarchical summary reports, like totals per product, per category, and an overall total, without writing separate queries for each level.

<a id="what-is-the-difference-between-group-by-and-using-a-window-function-for-aggregation"></a>
### Q: What is the difference between `GROUP BY` and using a window function for aggregation?
**Answer:** `GROUP BY` collapses multiple rows into one summary row per group, losing the original individual row detail. A window function computes an aggregate value across a group of related rows but still returns one row per original row, letting you see both the detail and an aggregate side by side.

<a id="how-would-you-find-duplicate-rows-in-a-table-based-on-a-specific-column"></a>
### Q: How would you find duplicate rows in a table based on a specific column?
**Answer:** Group by that column and filter with `HAVING COUNT(*) > 1`.

**Example:**
```sql
SELECT email, COUNT(*) AS cnt
FROM users
GROUP BY email
HAVING COUNT(*) > 1;
```

<a id="what-is-the-difference-between-sum-and-count-when-a-column-contains-null-values"></a>
### Q: What is the difference between `SUM()` and `COUNT()` when a column contains `NULL` values?
**Answer:** `SUM(column)` adds up only the non-`NULL` numeric values, ignoring `NULL`s entirely, treating them as if they weren't there rather than as zero. `COUNT(column)` counts only the rows where that column is non-`NULL`.

<a id="how-would-you-calculate-a-percentage-of-a-total-within-each-group-using-aggregation"></a>
### Q: How would you calculate a percentage of a total within each group using aggregation?
**Answer:** Compute each group's sum, divide by the grand total (often via a window function computing the overall sum), and multiply by 100.

**Example:**
```sql
SELECT category,
       SUM(amount) AS category_total,
       SUM(amount) * 100.0 / SUM(SUM(amount)) OVER () AS pct_of_total
FROM sales
GROUP BY category;
```

---

<a id="subqueries-ctes"></a>
## Subqueries & CTEs

<a id="what-is-a-subquery-and-where-can-it-be-used"></a>
### Q: What is a subquery, and where can it be used?
**Answer:** A query nested inside another SQL statement — it can appear in the `SELECT` list (a scalar subquery), the `FROM` clause (a derived table), or the `WHERE`/`HAVING` clause for filtering, depending on what it returns.

<a id="what-is-the-difference-between-a-correlated-and-non-correlated-subquery"></a>
### Q: What is the difference between a correlated and non-correlated subquery?
**Answer:** A non-correlated subquery is entirely self-contained and executes once, independent of the outer query. A correlated subquery references a column from the outer query, so conceptually it re-runs once per row processed by the outer query — often significantly more expensive on large datasets.

<a id="what-is-a-common-table-expression-cte-and-what-does-the-with-clause-do"></a>
### Q: What is a Common Table Expression (CTE), and what does the `WITH` clause do?
**Answer:** A CTE is a named, temporary result set defined at the start of a query using `WITH`, which can then be referenced like a regular table within the main query that follows — improving readability for complex queries by breaking them into named, logical steps.

**Example:**
```sql
WITH high_value_customers AS (
  SELECT customer_id, SUM(amount) AS total
  FROM orders
  GROUP BY customer_id
  HAVING SUM(amount) > 1000
)
SELECT * FROM high_value_customers;
```

<a id="what-is-a-recursive-cte-and-what-problem-does-it-solve"></a>
### Q: What is a recursive CTE, and what problem does it solve?
**Answer:** A CTE that references itself, letting you traverse hierarchical or graph-like data, like an org chart or a category tree, of unknown or variable depth — something a plain, non-recursive query structure can't easily express.

**Example:**
```sql
WITH RECURSIVE org_chart AS (
  SELECT id, name, manager_id FROM employees WHERE manager_id IS NULL
  UNION ALL
  SELECT e.id, e.name, e.manager_id
  FROM employees e
  JOIN org_chart o ON e.manager_id = o.id
)
SELECT * FROM org_chart;
```

<a id="what-is-the-difference-between-a-cte-and-a-subquery-in-the-from-clause"></a>
### Q: What is the difference between a CTE and a subquery in the `FROM` clause?
**Answer:** Functionally, a non-recursive CTE and an equivalent derived subquery often produce the same result, and depending on the database and query optimizer, may even execute identically. The main practical difference is readability and reusability — a CTE can be referenced multiple times within the same query by name.

<a id="what-is-the-difference-between-a-scalar-subquery-and-a-subquery-used-with-in"></a>
### Q: What is the difference between a scalar subquery and a subquery used with `IN`?
**Answer:** A scalar subquery must return exactly one column and one row (or `NULL`), usable anywhere a single value is expected, like in a `SELECT` list or an equality comparison. A subquery used with `IN` can return multiple rows of a single column, checked against for membership.

<a id="can-a-subquery-return-multiple-columns-and-where-would-that-be-valid"></a>
### Q: Can a subquery return multiple columns, and where would that be valid?
**Answer:** Yes — a subquery in the `FROM` clause (a derived table) can return any number of columns, since it's being treated as a full temporary table. Subqueries used in scalar contexts must return exactly one column, though multi-column comparisons are supported by some databases.

<a id="what-is-a-common-performance-concern-with-correlated-subqueries-and-how-might-you-rewrite-one-to-avoid-it"></a>
### Q: What is a common performance concern with correlated subqueries, and how might you rewrite one to avoid it?
**Answer:** A correlated subquery can effectively force a nested-loop-style re-execution once per outer row, which is slow at scale. It can often be rewritten as an equivalent `JOIN`, or a CTE combined with a join, letting the database's query planner potentially choose a more efficient join strategy instead.

<a id="what-is-the-difference-between-exists-and-in-in-terms-of-handling-null-values"></a>
### Q: What is the difference between `EXISTS` and `IN` in terms of handling `NULL` values?
**Answer:** `IN` can behave unexpectedly if the subquery's result list contains a `NULL` value — depending on the surrounding logic, especially with `NOT IN`, a `NULL` in the list can cause the entire condition to evaluate to unknown rather than the intended result. `EXISTS` doesn't have this pitfall, since it only checks for the presence of any matching row.

<a id="how-would-you-use-a-cte-to-simplify-a-query-that-otherwise-needs-a-subquery-repeated-multiple-times"></a>
### Q: How would you use a CTE to simplify a query that otherwise needs a subquery repeated multiple times?
**Answer:** Define the shared logic once as a named CTE at the top with `WITH`, then reference that CTE by name wherever the repeated subquery would have been used — avoiding duplicated logic, and potential inconsistency if one copy is edited but not the other, throughout the rest of the query.

---

<a id="indexes-query-optimization"></a>
## Indexes & Query Optimization

<a id="what-is-an-index-and-what-data-structure-do-most-databases-use-for-one"></a>
### Q: What is an index, and what data structure do most databases use for one?
**Answer:** An index is an auxiliary data structure that stores a sorted (or otherwise organized) reference to column values and pointers to their corresponding rows, letting the database avoid scanning the whole table to find matches. Most relational databases use a B-tree (or B+ tree) structure by default, supporting efficient lookups, range scans, and sorted retrieval.

<a id="what-is-the-difference-between-a-clustered-and-non-clustered-index"></a>
### Q: What is the difference between a clustered and non-clustered index?
**Answer:** A clustered index physically determines the order rows are stored on disk — a table can have only one, since data can only be sorted one physical way. A non-clustered index is a separate structure holding sorted key values with pointers back to the actual row location, and a table can have several of them.

<a id="what-is-a-composite-multi-column-index-and-does-column-order-matter"></a>
### Q: What is a composite (multi-column) index, and does column order matter?
**Answer:** An index built on multiple columns together. Order matters significantly — a composite index on `(a, b)` efficiently supports queries filtering on `a` alone, or on `a` AND `b` together, but generally can't efficiently support a query that filters only on `b` without `a`.

<a id="what-are-the-trade-offs-of-adding-more-indexes-to-a-table"></a>
### Q: What are the trade-offs of adding more indexes to a table?
**Answer:** Indexes speed up reads (`SELECT` queries filtering/sorting on indexed columns) but slow down writes (`INSERT`/`UPDATE`/`DELETE`), since every index must also be updated whenever the underlying data changes — and each index also consumes additional disk space.

<a id="what-is-the-explain-command-used-for"></a>
### Q: What is the `EXPLAIN` command used for?
**Answer:** It shows the database's query execution plan — how it intends to (or, with `EXPLAIN ANALYZE`, actually did) retrieve the data: which indexes were used or not, the join strategy chosen, estimated/actual row counts, and relative cost at each step — essential for diagnosing why a query is slow.

<a id="what-is-a-full-table-scan-and-why-is-it-usually-something-to-avoid-on-large-tables"></a>
### Q: What is a full table scan, and why is it usually something to avoid on large tables?
**Answer:** A full table scan reads every single row in a table to evaluate a query's condition, rather than using an index to jump directly to matching rows. On small tables this can actually be faster than using an index due to overhead, but on large tables it's typically far slower and a common sign that an appropriate index is missing.

<a id="what-is-index-selectivity-and-why-does-it-matter"></a>
### Q: What is index selectivity, and why does it matter?
**Answer:** Selectivity describes how many distinct values an indexed column has relative to the table's total row count. A highly selective column, like an email address nearly unique per row, makes for a very effective index. A low-selectivity column, like a boolean flag, provides much less benefit as an index on its own.

<a id="what-is-a-covering-index"></a>
### Q: What is a covering index?
**Answer:** An index that includes ALL the columns a particular query needs, both for filtering and for the columns being selected, letting the database satisfy the entire query directly from the index itself without a further lookup into the actual table data — significantly faster.

<a id="how-can-using-a-function-on-an-indexed-column-in-a-where-clause-hurt-performance"></a>
### Q: How can using a function on an indexed column in a `WHERE` clause hurt performance?
**Answer:** Wrapping an indexed column in a function, e.g. `WHERE UPPER(name) = 'JOHN'`, typically prevents the database from using a standard index on that column, since the stored index values don't match the transformed values being searched for — forcing a full scan unless a special function-based (expression) index is created specifically for that transformed expression.

<a id="what-is-query-plan-caching-and-why-does-it-matter-for-repeated-queries"></a>
### Q: What is query plan caching, and why does it matter for repeated queries?
**Answer:** Many databases cache the execution plan for a parameterized query after the first time it's compiled, reusing that plan for subsequent executions with different parameter values — avoiding the overhead of re-planning the same query structure repeatedly, though a cached plan optimized for one set of parameter values can occasionally be suboptimal for very different values later ("parameter sniffing").

---

<a id="normalization-database-design"></a>
## Normalization & Database Design

<a id="what-is-database-normalization-and-what-problem-does-it-solve"></a>
### Q: What is database normalization, and what problem does it solve?
**Answer:** Normalization organizes a database's tables and columns to reduce data redundancy and prevent inconsistent, anomalous updates, by splitting data into multiple related tables connected by foreign keys, following a structured series of rules called normal forms.

<a id="what-is-first-normal-form-1nf"></a>
### Q: What is First Normal Form (1NF)?
**Answer:** A table is in 1NF if each column holds only atomic (indivisible) values — no repeating groups or arrays crammed into a single column — and each row is uniquely identifiable.

<a id="what-is-second-normal-form-2nf"></a>
### Q: What is Second Normal Form (2NF)?
**Answer:** A table is in 2NF if it's already in 1NF, and every non-key column depends on the entire primary key, not just part of it — relevant specifically for tables with a composite (multi-column) primary key, where a partial dependency would violate 2NF.

<a id="what-is-third-normal-form-3nf"></a>
### Q: What is Third Normal Form (3NF)?
**Answer:** A table is in 3NF if it's already in 2NF, and it has no transitive dependencies — meaning non-key columns depend directly on the primary key, not indirectly through another non-key column.

<a id="what-are-insertion-update-and-deletion-anomalies-and-how-does-normalization-prevent-them"></a>
### Q: What are insertion, update, and deletion anomalies, and how does normalization prevent them?
**Answer:** An insertion anomaly happens when you can't add certain data without also having unrelated data available. An update anomaly happens when the same fact is duplicated across many rows, risking inconsistency if only some copies get updated. A deletion anomaly happens when removing one record accidentally destroys other, unrelated information stored in the same row. Normalization prevents all three by separating distinct facts into their own appropriately-scoped tables.

<a id="what-is-denormalization-and-why-might-you-intentionally-denormalize-a-database"></a>
### Q: What is denormalization, and why might you intentionally denormalize a database?
**Answer:** Denormalization deliberately introduces some redundancy, often by combining tables or duplicating data, to improve read performance, typically by avoiding expensive joins for very frequently-run queries — a trade-off accepting more complex/careful writes in exchange for faster reads, common in reporting/analytics systems.

<a id="what-is-a-composite-key"></a>
### Q: What is a composite key?
**Answer:** A primary key made up of two or more columns together, where the combination of those columns is what's guaranteed unique, even if no single column alone is — common in junction/join tables representing many-to-many relationships.

<a id="what-is-a-surrogate-key-and-how-does-it-differ-from-a-natural-key"></a>
### Q: What is a surrogate key, and how does it differ from a natural key?
**Answer:** A surrogate key is an artificially generated identifier, like an auto-incrementing integer or a UUID, with no inherent business meaning, used purely to uniquely identify a row. A natural key is derived from actual real-world data that's already unique, like a national ID number — surrogate keys are generally preferred since natural keys can sometimes change or turn out not to be as unique as assumed.

<a id="what-is-an-entity-relationship-er-diagram-and-why-is-it-useful-in-database-design"></a>
### Q: What is an Entity-Relationship (ER) diagram, and why is it useful in database design?
**Answer:** A visual diagram representing a database's entities (tables), their attributes (columns), and the relationships between them — one-to-one, one-to-many, many-to-many — used as a planning and communication tool before physically implementing a schema, helping catch design issues early.

<a id="when-might-you-choose-to-design-a-table-with-a-many-to-many-relationship-and-how-do-you-implement-it-in-sql"></a>
### Q: When might you choose to design a table with a many-to-many relationship, and how do you implement it in SQL?
**Answer:** When two entities can each be associated with multiple instances of the other, e.g. students can enroll in many courses and each course has many students. It's implemented with a separate junction (or "bridge") table holding foreign keys referencing both related tables, typically with a composite primary key across those two foreign key columns.

---

<a id="constraints-keys"></a>
## Constraints & Keys

<a id="what-is-a-primary-key-constraint-and-what-does-it-enforce"></a>
### Q: What is a `PRIMARY KEY` constraint, and what does it enforce?
**Answer:** It uniquely identifies each row in a table, enforcing both uniqueness (no two rows can share the same value) and non-nullability (the column can't be `NULL`) — a table can have only one primary key, though it can span multiple columns as a composite key.

<a id="what-is-a-foreign-key-constraint-and-what-does-it-enforce"></a>
### Q: What is a `FOREIGN KEY` constraint, and what does it enforce?
**Answer:** It links a column in one table to the primary key (or a unique key) of another table, enforcing referential integrity — you can't insert a row with a foreign key value that doesn't exist in the referenced table.

<a id="what-is-a-unique-constraint-and-how-does-it-differ-from-a-primary-key"></a>
### Q: What is a `UNIQUE` constraint, and how does it differ from a `PRIMARY KEY`?
**Answer:** `UNIQUE` ensures no two rows have the same value in that column (or combination of columns), similar to a primary key, but a table can have multiple `UNIQUE` constraints, and in most databases a `UNIQUE` column can allow `NULL` values, unlike a `PRIMARY KEY`.

<a id="what-is-a-check-constraint"></a>
### Q: What is a `CHECK` constraint?
**Answer:** A rule that restricts what values are allowed in a column, evaluated as a boolean expression that must be true for every row — e.g. `CHECK (age >= 0)` prevents negative ages from ever being inserted or updated into that column.

<a id="what-is-a-not-null-constraint"></a>
### Q: What is a `NOT NULL` constraint?
**Answer:** It requires that a column must always have a value — attempting to insert or update a row leaving that column as `NULL` will be rejected by the database.

<a id="what-does-on-delete-cascade-do-on-a-foreign-key"></a>
### Q: What does `ON DELETE CASCADE` do on a foreign key?
**Answer:** It automatically deletes any child rows referencing a parent row when that parent row is deleted, keeping referential integrity intact automatically rather than requiring the application to manually clean up dependent rows first.

<a id="what-is-the-difference-between-on-delete-cascade-on-delete-set-null-and-on-delete-restrict"></a>
### Q: What is the difference between `ON DELETE CASCADE`, `ON DELETE SET NULL`, and `ON DELETE RESTRICT`?
**Answer:** `CASCADE` deletes dependent child rows along with the parent. `SET NULL` keeps the child rows but sets their foreign key column to `NULL`, only valid if that column is nullable. `RESTRICT`, or the default behavior in many databases, simply prevents the parent row from being deleted at all while dependent child rows still reference it.

<a id="what-is-a-default-constraint"></a>
### Q: What is a `DEFAULT` constraint?
**Answer:** It specifies a value to automatically use for a column when an `INSERT` statement doesn't explicitly provide one — e.g. a `created_at` column defaulting to the current timestamp automatically stamps a row's creation time without the application needing to supply it.

---

<a id="transactions-acid"></a>
## Transactions & ACID

<a id="what-is-a-database-transaction"></a>
### Q: What is a database transaction?
**Answer:** A sequence of one or more SQL statements executed together as a single, indivisible logical unit — either every statement in it takes effect via `COMMIT`, or none of them do via `ROLLBACK`, even if the database crashes partway through.

<a id="what-does-acid-stand-for-and-briefly-explain-each-property"></a>
### Q: What does ACID stand for, and briefly explain each property.
**Answer:** Atomicity (a transaction is all-or-nothing), Consistency (a transaction moves the database from one valid state to another, respecting all constraints/rules), Isolation (concurrently running transactions don't see each other's uncommitted intermediate changes), and Durability (once a transaction commits, its changes persist even through a subsequent crash or power failure).

<a id="what-is-the-difference-between-commit-and-rollback"></a>
### Q: What is the difference between `COMMIT` and `ROLLBACK`?
**Answer:** `COMMIT` permanently saves all changes made during the current transaction, making them visible to other sessions/transactions. `ROLLBACK` discards all changes made during the current transaction, reverting the database to the state it was in before the transaction began.

<a id="what-is-a-savepoint-and-why-would-you-use-one"></a>
### Q: What is a `SAVEPOINT`, and why would you use one?
**Answer:** A named point within a larger transaction that you can later roll back to, without undoing the entire transaction — useful when you want the option to discard just part of a multi-step transaction's work while keeping earlier steps intact.

<a id="what-are-the-standard-transaction-isolation-levels-from-least-to-most-strict"></a>
### Q: What are the standard transaction isolation levels, from least to most strict?
**Answer:** `READ UNCOMMITTED` (can see other transactions' uncommitted changes, "dirty reads"), `READ COMMITTED` (only sees committed data, but values can change between repeated reads in the same transaction), `REPEATABLE READ` (repeated reads within the same transaction see consistent values), and `SERIALIZABLE` (the strictest — transactions behave as if fully executed one after another, with no concurrency-related anomalies).

<a id="what-is-a-dirty-read"></a>
### Q: What is a dirty read?
**Answer:** When a transaction reads data that another, still-uncommitted transaction has changed — if that other transaction later rolls back, the first transaction ends up having read data that technically never really existed in a committed state.

<a id="what-is-a-non-repeatable-read"></a>
### Q: What is a non-repeatable read?
**Answer:** When a transaction reads the same row twice and gets different values each time, because another transaction committed a change to that row in between the two reads — possible under `READ COMMITTED` isolation but prevented by `REPEATABLE READ` and stricter levels.

<a id="what-is-a-phantom-read"></a>
### Q: What is a phantom read?
**Answer:** When a transaction re-runs the same query twice and gets a different set of rows the second time, not just different values in existing rows, because another transaction inserted or deleted rows matching that query's condition in between — prevented only at the `SERIALIZABLE` isolation level in most databases.

<a id="what-is-a-deadlock-and-how-do-databases-typically-handle-one"></a>
### Q: What is a deadlock, and how do databases typically handle one?
**Answer:** A deadlock occurs when two or more transactions each hold a lock the other needs, and each is waiting for the other to release theirs — neither can ever proceed. Most databases automatically detect this situation and forcibly roll back one of the transactions (the "victim"), returning an error so the application can retry.

<a id="what-is-optimistic-locking-and-how-does-it-differ-from-pessimistic-locking"></a>
### Q: What is optimistic locking, and how does it differ from pessimistic locking?
**Answer:** Pessimistic locking acquires a lock on data upfront before making changes, blocking other transactions from touching it in the meantime. Optimistic locking instead allows concurrent access without locking upfront, and checks, often via a version number or timestamp column, at update time whether the data changed since it was read — failing the update if a conflict is detected, rather than blocking other transactions preemptively.

---

<a id="window-functions"></a>
## Window Functions

<a id="what-is-a-window-function-and-how-does-it-differ-from-a-regular-aggregate-function-used-with-group-by"></a>
### Q: What is a window function, and how does it differ from a regular aggregate function used with `GROUP BY`?
**Answer:** A window function computes a value across a set (a "window") of related rows, similar to an aggregate function, but without collapsing those rows into a single output row — every original row is still returned individually, now with the computed window value alongside it.

<a id="what-does-the-over-clause-do"></a>
### Q: What does the `OVER()` clause do?
**Answer:** It turns a function into a window function and defines the window of rows it operates over — which can be the entire result set, a partition of it via `PARTITION BY`, and/or ordered in a particular way via `ORDER BY` within the `OVER` clause.

**Example:**
```sql
SELECT name, department, salary,
       AVG(salary) OVER (PARTITION BY department) AS dept_avg
FROM employees;
```

<a id="what-is-the-difference-between-rank-denserank-and-rownumber"></a>
### Q: What is the difference between `RANK()`, `DENSE_RANK()`, and `ROW_NUMBER()`?
**Answer:** `ROW_NUMBER()` assigns a unique, sequential number to each row within its window, with no gaps or ties, even if values are identical. `RANK()` gives tied rows the same rank, but then skips the next rank number(s) accordingly, e.g. 1, 2, 2, 4. `DENSE_RANK()` also gives tied rows the same rank, but does not skip subsequent numbers, e.g. 1, 2, 2, 3.

<a id="what-does-partition-by-do-within-a-window-function-and-how-does-it-differ-from-group-by"></a>
### Q: What does `PARTITION BY` do within a window function, and how does it differ from `GROUP BY`?
**Answer:** `PARTITION BY` divides the rows into separate groups for the purposes of the window function's calculation, similar in concept to `GROUP BY`, but unlike `GROUP BY`, it doesn't collapse the rows in the final output; each original row remains present, just annotated with a value computed within its own partition.

<a id="what-are-the-lag-and-lead-functions-used-for"></a>
### Q: What are the `LAG()` and `LEAD()` functions used for?
**Answer:** `LAG()` retrieves a column's value from a previous row within the window, a specified number of rows back, default 1. `LEAD()` retrieves a value from a following row. Both are commonly used to compare a row to its neighbor, like calculating month-over-month change.

**Example:**
```sql
SELECT month, revenue,
       LAG(revenue) OVER (ORDER BY month) AS prev_month_revenue
FROM monthly_sales;
```

<a id="what-is-the-difference-between-ntilen-and-rank"></a>
### Q: What is the difference between `NTILE(n)` and `RANK()`?
**Answer:** `NTILE(n)` divides the rows in a window into `n` roughly equal-sized buckets, like quartiles with `NTILE(4)`, and assigns each row its bucket number. `RANK()` instead assigns a positional rank based purely on ordering, with ties handled by skipping subsequent rank numbers — the two serve different purposes, bucketing vs. strict ordering.

<a id="how-would-you-calculate-a-running-total-using-a-window-function"></a>
### Q: How would you calculate a running total using a window function?
**Answer:** Use `SUM()` as a window function ordered by the relevant column, with the default frame extending from the start of the partition up to the current row.

**Example:**
```sql
SELECT order_date, amount,
       SUM(amount) OVER (ORDER BY order_date) AS running_total
FROM orders;
```

<a id="what-is-a-window-frame-and-how-do-rows-between-and-range-between-differ"></a>
### Q: What is a window frame, and how do `ROWS BETWEEN` and `RANGE BETWEEN` differ?
**Answer:** A window frame defines exactly which rows, relative to the current row, are included in the window function's calculation. `ROWS BETWEEN` counts a specific number of physical rows before/after. `RANGE BETWEEN` instead includes all rows within a specified logical value range relative to the current row's `ORDER BY` value, which can include a different number of actual rows if there are ties.

<a id="can-you-use-a-window-functions-result-directly-in-a-where-clause"></a>
### Q: Can you use a window function's result directly in a `WHERE` clause?
**Answer:** No — window functions are logically evaluated after `WHERE`, and even after `GROUP BY`/`HAVING`, so you can't filter on a window function's result directly in the same query's `WHERE` clause. You'd need to wrap the query in a subquery or CTE and filter in the outer query instead.

<a id="how-would-you-find-for-each-department-the-employee-with-the-highest-salary-using-a-window-function"></a>
### Q: How would you find, for each department, the employee with the highest salary using a window function?
**Answer:** Rank employees within each department by salary using `ROW_NUMBER()` partitioned by department, then filter in an outer query to just the rows ranked first.

**Example:**
```sql
SELECT * FROM (
  SELECT *, ROW_NUMBER() OVER (PARTITION BY department ORDER BY salary DESC) AS rn
  FROM employees
) ranked
WHERE rn = 1;
```

---

<a id="views-stored-procedures-triggers"></a>
## Views, Stored Procedures & Triggers

<a id="what-is-a-view-and-what-are-its-main-benefits"></a>
### Q: What is a view, and what are its main benefits?
**Answer:** A view is a saved, named query that behaves like a virtual table — you can `SELECT` from it, and sometimes update through it, just like a regular table. Benefits include simplifying complex/repeated queries, restricting which underlying columns/rows a user can see, and providing a stable interface even if the underlying table structure changes.

<a id="what-is-the-difference-between-a-regular-view-and-a-materialized-view"></a>
### Q: What is the difference between a regular view and a materialized view?
**Answer:** A regular view re-runs its underlying query fresh every time it's queried, always reflecting current data but with no storage or performance saved compared to running the query directly. A materialized view physically stores its result set on disk, making reads much faster, but that stored data becomes stale until the materialized view is explicitly refreshed.

<a id="what-is-a-stored-procedure-and-what-are-its-advantages"></a>
### Q: What is a stored procedure, and what are its advantages?
**Answer:** A stored procedure is a precompiled, named set of SQL statements, often with parameters and control-flow logic, saved in the database and callable as a single unit. Advantages: reduced network round-trips, centralized/reusable business logic, and often better performance since the execution plan can be cached.

<a id="what-is-the-difference-between-a-stored-procedure-and-a-function-in-sql"></a>
### Q: What is the difference between a stored procedure and a function in SQL?
**Answer:** A stored procedure can perform actions, including DML like `INSERT`/`UPDATE`, doesn't have to return a value, and is invoked with a `CALL`/`EXEC` statement. A function must return a single value or table, generally can't perform data-modifying side effects in most databases, and can be used directly within a `SELECT` statement's expression, unlike a stored procedure.

<a id="what-is-a-trigger-and-what-are-common-events-that-can-fire-one"></a>
### Q: What is a trigger, and what are common events that can fire one?
**Answer:** A trigger is a piece of code automatically executed by the database in response to a specific event on a table — typically `BEFORE`/`AFTER` an `INSERT`, `UPDATE`, or `DELETE` — used for tasks like maintaining an audit log, enforcing complex business rules, or keeping denormalized/derived data in sync.

<a id="what-is-a-potential-downside-of-relying-heavily-on-triggers"></a>
### Q: What is a potential downside of relying heavily on triggers?
**Answer:** Triggers can make application behavior harder to trace and debug, since side effects happen implicitly inside the database rather than explicitly in application code — a developer looking only at the application layer might be completely unaware that a certain update also silently modifies other tables via a trigger.

<a id="can-a-view-be-updated-and-what-conditions-typically-need-to-be-met"></a>
### Q: Can a view be updated, and what conditions typically need to be met?
**Answer:** Some views are updatable, meaning writes through the view actually modify the underlying base table, but generally only if the view is based on a single table, doesn't use aggregate functions, `GROUP BY`, `DISTINCT`, or set operations, and includes any columns required by the base table's constraints.

<a id="what-is-the-difference-between-before-and-after-triggers"></a>
### Q: What is the difference between `BEFORE` and `AFTER` triggers?
**Answer:** A `BEFORE` trigger runs prior to the triggering operation actually being applied, letting it validate or even modify the incoming data before it's written. An `AFTER` trigger runs once the operation has already completed, typically used for logging or cascading follow-up actions that depend on the change already having taken effect.

---

<a id="common-coding-challenges"></a>
## Common Coding Challenges

<a id="write-a-query-to-find-the-second-highest-salary-in-a-table"></a>
### Q: Write a query to find the second-highest salary in a table.
**Answer:** Filter for the maximum salary that's still less than the overall maximum.

**Example:**
```sql
SELECT MAX(salary) AS second_highest
FROM employees
WHERE salary < (SELECT MAX(salary) FROM employees);
```

<a id="write-a-query-to-find-duplicate-email-addresses-in-a-users-table"></a>
### Q: Write a query to find duplicate email addresses in a users table.
**Answer:** Group by the email column and filter to groups with more than one row.

**Example:**
```sql
SELECT email, COUNT(*) AS occurrences
FROM users
GROUP BY email
HAVING COUNT(*) > 1;
```

<a id="write-a-query-to-find-employees-who-earn-more-than-their-manager"></a>
### Q: Write a query to find employees who earn more than their manager.
**Answer:** Self-join the employees table so each employee row is paired with their manager's row, then compare salaries.

**Example:**
```sql
SELECT e.name AS employee, m.name AS manager
FROM employees e
JOIN employees m ON e.manager_id = m.id
WHERE e.salary > m.salary;
```

<a id="write-a-query-to-delete-duplicate-rows-keeping-only-one-copy-of-each"></a>
### Q: Write a query to delete duplicate rows, keeping only one copy of each.
**Answer:** Keep the row with the minimum ID per duplicate group, and delete everything else sharing that group's key.

**Example:**
```sql
DELETE FROM users
WHERE id NOT IN (
  SELECT MIN(id)
  FROM users
  GROUP BY email
);
```

<a id="write-a-query-to-find-the-nth-highest-salary-using-a-window-function"></a>
### Q: Write a query to find the Nth highest salary using a window function.
**Answer:** Rank distinct salaries in descending order with `DENSE_RANK()`, then filter to the desired rank.

**Example:**
```sql
SELECT DISTINCT salary
FROM (
  SELECT salary, DENSE_RANK() OVER (ORDER BY salary DESC) AS rnk
  FROM employees
) ranked
WHERE rnk = 3; -- 3rd highest
```

<a id="write-a-query-to-calculate-month-over-month-percentage-growth-in-revenue"></a>
### Q: Write a query to calculate month-over-month percentage growth in revenue.
**Answer:** Use `LAG()` to pull the previous month's revenue alongside the current row, then compute the percentage change.

**Example:**
```sql
SELECT month,
       revenue,
       (revenue - LAG(revenue) OVER (ORDER BY month)) * 100.0
         / LAG(revenue) OVER (ORDER BY month) AS pct_growth
FROM monthly_revenue;
```

<a id="write-a-query-using-a-recursive-cte-to-find-all-subordinates-under-a-given-manager"></a>
### Q: Write a query using a recursive CTE to find all subordinates under a given manager.
**Answer:** Start with the given manager as the anchor member, then recursively join employees whose manager_id matches someone already found.

**Example:**
```sql
WITH RECURSIVE subordinates AS (
  SELECT id, name, manager_id FROM employees WHERE id = 1
  UNION ALL
  SELECT e.id, e.name, e.manager_id
  FROM employees e
  JOIN subordinates s ON e.manager_id = s.id
)
SELECT * FROM subordinates;
```

<a id="write-a-query-to-pivot-rows-into-columns-eg-showing-total-sales-per-quarter-as-separate-columns"></a>
### Q: Write a query to pivot rows into columns, e.g. showing total sales per quarter as separate columns.
**Answer:** Use conditional aggregation with `CASE` expressions inside `SUM()`, one per desired output column.

**Example:**
```sql
SELECT
  SUM(CASE WHEN quarter = 'Q1' THEN amount ELSE 0 END) AS q1,
  SUM(CASE WHEN quarter = 'Q2' THEN amount ELSE 0 END) AS q2,
  SUM(CASE WHEN quarter = 'Q3' THEN amount ELSE 0 END) AS q3,
  SUM(CASE WHEN quarter = 'Q4' THEN amount ELSE 0 END) AS q4
FROM sales;
```

<a id="write-a-query-to-find-customers-who-have-never-placed-an-order"></a>
### Q: Write a query to find customers who have never placed an order.
**Answer:** Left join customers to orders and filter to rows where no matching order was found.

**Example:**
```sql
SELECT c.*
FROM customers c
LEFT JOIN orders o ON c.id = o.customer_id
WHERE o.id IS NULL;
```

<a id="write-a-query-to-find-the-top-3-products-by-total-revenue"></a>
### Q: Write a query to find the top 3 products by total revenue.
**Answer:** Compute revenue per product by aggregating order items, then sort descending and limit to 3.

**Example:**
```sql
SELECT product_id, SUM(quantity * price) AS revenue
FROM order_items
GROUP BY product_id
ORDER BY revenue DESC
LIMIT 3;
```

---

<a id="behavioral-scenario-based-questions"></a>
## Behavioral / Scenario-Based Questions

<a id="how-would-you-approach-optimizing-a-slow-running-query-in-production"></a>
### Q: How would you approach optimizing a slow-running query in production?
**Answer:** Run `EXPLAIN`/`EXPLAIN ANALYZE` to see the actual query plan, check whether relevant columns (join conditions, `WHERE` filters, `ORDER BY`) are indexed, look for full table scans or inefficient nested-loop joins on large tables, consider rewriting correlated subqueries as joins, and verify statistics are up to date so the query planner has accurate information to work with.

<a id="how-would-you-design-a-database-schema-for-an-e-commerce-platforms-orders-and-products"></a>
### Q: How would you design a database schema for an e-commerce platform's orders and products?
**Answer:** Separate core entities into their own tables — customers, products, orders, and a junction table like order_items linking orders to products, since one order can contain many products and a product can appear in many orders — using foreign keys to maintain referential integrity, and indexing frequently-queried/joined columns like customer_id and product_id.

<a id="how-would-you-handle-a-situation-where-two-transactions-are-deadlocking-each-other-in-production"></a>
### Q: How would you handle a situation where two transactions are deadlocking each other in production?
**Answer:** Rely on the database's automatic deadlock detection to roll back one transaction, but investigate the actual application code causing it, commonly caused by two transactions acquiring the same set of locks in a different order, and fix it by enforcing a consistent lock-acquisition order across the codebase, or reducing transaction scope/duration.

<a id="how-would-you-decide-between-normalizing-and-denormalizing-a-particular-part-of-a-schema"></a>
### Q: How would you decide between normalizing and denormalizing a particular part of a schema?
**Answer:** Consider the read/write ratio and query patterns for that specific data — normalize by default for data integrity and to avoid update anomalies, but consider selectively denormalizing for a specific, well-understood hot path where join/aggregation performance genuinely can't keep up otherwise, accepting the added complexity of keeping duplicated data in sync.

<a id="how-would-you-migrate-a-large-production-tables-schema-eg-adding-a-new-column-with-minimal-downtime"></a>
### Q: How would you migrate a large production table's schema, e.g. adding a new column, with minimal downtime?
**Answer:** Depending on the database, use online/concurrent schema-change features if available rather than a blocking `ALTER TABLE` on a huge table, add new columns as nullable or with a cheap default first, backfill data in small batches to avoid long-running locks, and only add stricter constraints like `NOT NULL` once the backfill is fully complete and verified.

<a id="how-would-you-investigate-data-inconsistency-between-two-related-tables-that-should-always-stay-in-sync"></a>
### Q: How would you investigate data inconsistency between two related tables that should always stay in sync?
**Answer:** Write a query joining the two tables, often a `LEFT JOIN` in both directions, to surface any orphaned or mismatched rows, check whether the relevant foreign key constraints are actually enforced or missing, and review the application/trigger logic responsible for keeping both tables updated together to find where they can drift apart.

<a id="how-would-you-choose-between-using-a-stored-procedure-and-handling-logic-in-the-application-code"></a>
### Q: How would you choose between using a stored procedure and handling logic in the application code?
**Answer:** Consider team familiarity and tooling, since stored procedures can be harder to version-control, test, and debug compared to application code, performance-critical paths where reducing round-trips matters significantly, and whether the logic genuinely needs to run close to the data versus logic that's more naturally expressed and maintained in the application layer.

<a id="how-would-you-approach-reviewing-a-teammates-sql-migration-or-query-in-a-code-review"></a>
### Q: How would you approach reviewing a teammate's SQL migration or query in a code review?
**Answer:** Check that new columns/tables have appropriate constraints and indexes, verify large migrations won't lock a production table for an unacceptable amount of time, look for missing `WHERE` clauses on `UPDATE`/`DELETE` statements, confirm joins use proper `ON` conditions rather than an accidental cross join, and check whether the query has been tested against realistic data volumes.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview?** Go section by section, top to bottom — each one builds on the last, from basics to window functions and architecture.
- **Revising the night before?** Jump straight to 🔥 Most Asked / Tricky Questions, then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
