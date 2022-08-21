## SQL & Cockroach

```
cockroach sql --url "<connection-string>"
show databases;
create database <database-name>
use <database-name>
show tables;
\d <table-name>

```

## Concepts
 - Primary key - Create random(No auto increment key) and strong key for distributed database to avoid hot spot.
 - Natural key
 - Surrogate key
 - Compound key - To minimize hot spot.
 - Hash feature(CockroachDB) to convert natural key to distribute across the cluster.
  - Bulk insert - Smaller chunk approach
  - Limit & Where(contains predicate) clause
  - Like, In, Comparision, >, <, >=, <= operators
  - Logical operators - AND, OR, NOT
  - Cockroach prevents query from executing if query doesn't have WHERE clause.
  - Bulk update - Smaller chunk approach
  - Deleted records would be garbage colleted with TTL.
  - Indexes - Primary and secondary index
  - Composite indexes - uses multiple column
  - Table scans - Use 'EXPLAIN' on query to find out if the table need on index.