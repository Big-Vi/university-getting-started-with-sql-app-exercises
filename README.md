## SQL & Cockroach

```
cockroach sql --url "<connection-string>"
show databases;
create database <database-name>
use <database-name>
show tables;

```

## Concepts
 - Primary key - Create random(No auto increment key) and strong key for distributed database to avoid hot spot.
 - Natural key
 - Surrogate key
 - Compound key - To minimize hot spot.
 - Hash feature(CockroachDB) to convert natural key to distribute across the cluster.
 