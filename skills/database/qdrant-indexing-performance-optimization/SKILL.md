---
name: 'qdrant-indexing-performance-optimization'
description: 'Diagnoses and fixes slow Qdrant indexing and data ingestion. Use when someone reports'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# qdrant-indexing-performance-optimization

"Diagnoses and fixes slow Qdrant indexing and data ingestion. Use when someone reports 'uploads are slow', 'indexing takes forever', 'optimizer is stuck', 'HNSW build time too long', or 'data uploaded

## When to Use

- Use this skill when working on tasks related to qdrant indexing performance optimization
- Apply best practices from awesome-copilot

## Workflow

name: qdrant-indexing-performance-optimization
description: "Diagnoses and fixes slow Qdrant indexing and data ingestion. Use when someone reports 'uploads are slow', 'indexing takes forever', 'optimizer is stuck', 'HNSW build time too long', or 'data uploaded but search is bad'. Also use when optimizer status shows errors, segments won't merge, or indexing threshold questions arise."
# What to Do When Qdrant Indexing Is Too Slow
Qdrant does NOT build HNSW indexes immediately. Small segments use brute-force until they exceed `indexing_threshold_kb` (default: 20 MB). Search during this window i

## Source

Adopted from: awesome-copilot
