---
name: 'sql-optimization'
description: 'Universal SQL performance optimization assistant for comprehensive query tuning, indexing strategies, and database performance analysis across all SQL databases (MySQL, PostgreSQL, SQL Server, Oracle'
version: 1.0.0
source: awesome-copilot
tier: 2
adopted: 2026-05-16
---

# sql-optimization

'Universal SQL performance optimization assistant for comprehensive query tuning, indexing strategies, and database performance analysis across all SQL databases (MySQL, PostgreSQL, SQL Server, Oracle

## When to Use

- Use this skill when working on tasks related to sql optimization
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: sql-optimization
description: 'Universal SQL performance optimization assistant for comprehensive query tuning, indexing strategies, and database performance analysis across all SQL databases (MySQL, PostgreSQL, SQL Server, Oracle). Provides execution plan analysis, pagination optimization, batch operations, and performance monitoring guidance.'
# SQL Performance Optimization Assistant
Expert SQL performance optimization for ${selection} (or entire project if no selection). Focus on universal SQL optimization techniques that work across MySQL, PostgreSQL, SQL Server, Oracle, and other SQL databases.
## 🎯 Core Optimization Areas
### Query Performance Analysis
```sql
-- ❌ BAD: Inefficient query patterns
SELECT * FROM orders o
WHERE YEAR(o.created_at) = 2024
  AND o.customer_id IN (
      SELECT c.id FROM customers c WHERE c.status = 'active'
  );
-- ✅ GOOD: Optimized query with proper indexing hints
SELECT o.id, o.customer_id, o.total_amount, o.created_at
FROM orders o
INNER JOIN customers c ON o.customer_id = c.id
WHERE o.created_at >= '2024-01-01' 
  AND o.created_at < '2025-01-01'
  AND c.status = 'active';

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: sql-optimization
