# CS304 — Database Systems (Advanced) — PLAN

**Semester:** 3 · **Credits:** 4 · **Level:** Intermediate-Advanced
**Theory:** 45 hrs · **Lab:** 30 hrs · **Tools:** PostgreSQL, MySQL, SQLite, Python, psycopg2

## Syllabus

### Unit 1 — Relational Theory and Advanced SQL (9 lectures)
1. Relational algebra recap — select, project, join
2. Relational calculus — tuple and domain
3. Schema refinement — normalisation to BCNF
4. Multivalued dependencies and 4NF
5. Join dependencies and 5NF
6. Advanced SQL — recursive CTEs
7. Advanced SQL — window functions deep dive
8. Advanced SQL — LATERAL joins and set-returning functions
9. Advanced SQL — stored procedures and triggers

### Unit 2 — Storage, Indexing, and Query Processing (9 lectures)
1. Storage hierarchy — disks, SSD, buffers
2. File organisation — heap, sorted, clustered
3. B-tree and B+ tree indexes
4. Hash indexes
5. Bitmap and covering indexes
6. Query processing — parsing, planning, execution
7. Cost estimation and statistics
8. Join algorithms — nested loop, hash, sort-merge
9. Query optimisation — rules and cost-based

### Unit 3 — Transactions and Concurrency (9 lectures)
1. Transactions — ACID revisited
2. Schedules — serial, serialisable, conflict-serialisable
3. Conflict serialisability and precedence graphs
4. Two-phase locking (2PL)
5. Strict 2PL, rigorous 2PL
6. Timestamp ordering and optimistic concurrency
7. Multi-version concurrency control (MVCC)
8. Isolation levels — read committed, repeatable read, serialisable
9. Phantom reads and predicate locking

### Unit 4 — Recovery, Security, and Administration (9 lectures)
1. Failure types — transaction, system, media
2. Write-ahead logging (WAL)
3. Undo/redo logging
4. Checkpoints and ARIES algorithm
5. Crash recovery in PostgreSQL (WAL, checkpoints)
6. Database users and privileges
7. Role-based access control
8. SQL injection — attacks and prevention
9. Backup strategies and point-in-time recovery

### Unit 5 — Distributed and NoSQL Databases (9 lectures)
1. Distributed databases — motivation and trade-offs
2. Replication — master-slave, master-master
3. Partitioning and sharding
4. CAP theorem
5. NoSQL categories — document, key-value, column, graph
6. MongoDB basics — documents and queries
7. Redis — in-memory data structures
8. Consistency models — strong, eventual, causal
9. NewSQL and modern distributed SQL (CockroachDB, Spanner)

## Practical Labs (18)

1. Set up PostgreSQL, connect with psql and Python
2. Write 10 advanced SQL queries using CTEs
3. Window functions — running totals, rankings, moving averages
4. Recursive CTE — organisational hierarchy
5. Trigger — audit log on INSERT/UPDATE
6. Stored procedure — daily summary report
7. Create and analyse a B-tree index
8. Compare query plans before and after indexing with `EXPLAIN ANALYZE`
9. Hash index vs B-tree — storage and lookup benchmarks
10. EXPLAIN ANALYZE on a multi-table join
11. Simulate a transaction and demonstrate rollback
12. Demonstrate isolation levels with two concurrent sessions
13. Detect a deadlock — read the PostgreSQL log
14. WAL inspection — read a checkpoint entry
15. Backup and restore — full and point-in-time
16. SQL injection — demonstrate vulnerable vs parameterised query
17. Connect to MongoDB and run CRUD operations
18. Set up Redis and implement a caching pattern

## Assignments

1. Schema design — a complete 3NF schema for a medium-sized domain
2. Advanced SQL — 15 query exercises
3. Query optimisation — rewrite five slow queries
4. Transaction analysis — 5 concurrent schedules
5. NoSQL comparison — model the same dataset in SQL and MongoDB
