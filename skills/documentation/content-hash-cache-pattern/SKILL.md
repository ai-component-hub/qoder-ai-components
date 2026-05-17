---
name: 'content-hash-cache-pattern'
description: 'Cache expensive file processing results using SHA-256 content hashes'
adopted: 2026-05-16
— path-independent, auto-invalidating, with service layer separation.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# content-hash-cache-pattern

Cache expensive file processing results using SHA-256 content hashes — path-independent, auto-invalidating, with service layer separation.

## When to Use

- Use this skill when working on tasks related to content hash cache pattern
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: content-hash-cache-pattern
description: Cache expensive file processing results using SHA-256 content hashes — path-independent, auto-invalidating, with service layer separation.
origin: ECC
# Content-Hash File Cache Pattern
Cache expensive file processing results (PDF parsing, text extraction, image analysis) using SHA-256 content hashes as cache keys. Unlike path-based caching, this approach survives file moves/renames and auto-invalidates when content changes.
## When to Activate
- Building file processing pipelines (PDF, images, text extraction)
- Processing cost is high and same files are processed repeatedly
- Need a `--cache/--no-cache` CLI option
- Want to add caching to existing pure functions without modifying them
## Core Pattern
### 1. Content-Hash Based Cache Key
Use file content (not path) as the cache key:
```python
import hashlib
from pathlib import Path
_HASH_CHUNK_SIZE = 65536  # 64KB chunks for large files
def compute_file_hash(path: Path) -> str:
    """SHA-256 of file contents (chunked for large files)."""
    if not path.is_file():

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: content-hash-cache-pattern
