+++
title = "duckdb_fdw"
description = "DuckDB Foreign Data Wrapper for PostgreSQL — 406⭐"
repo = "https://github.com/alitrack/duckdb_fdw"
lang = "C"
+++

让 PostgreSQL 直接查询 DuckDB 数据库的外包装。一条 SQL 跨越 OLTP 和 OLAP。

```sql
CREATE EXTENSION duckdb_fdw;
CREATE SERVER duckdb_server FOREIGN DATA WRAPPER duckdb_fdw;
CREATE FOREIGN TABLE analytics (...) SERVER duckdb_server;

-- 跨数据库 JOIN
SELECT * FROM transactions t
JOIN analytics a ON t.id = a.transaction_id;
```

被收录入 PostgreSQL 扩展名录，全球 30+ 贡献者。
