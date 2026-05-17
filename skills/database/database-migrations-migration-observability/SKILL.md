---
name: 'database-migrations-migration-observability'
description: 'Migration monitoring, CDC, and observability infrastructure'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# database-migrations-migration-observability

"Migration monitoring, CDC, and observability infrastructure"

## When to Use

- Use this skill when working on tasks related to database migrations migration observability
- Apply best practices from antigravity-awesome-skills

## Workflow

### 1. Observable MongoDB Migrations

```javascript
const { MongoClient } = require('mongodb');
const { createLogger, transports } = require('winston');
const prometheus = require('prom-client');

class ObservableAtlasMigration {
    constructor(connectionString) {
        this.client = new MongoClient(connectionString);
        this.logger = createLogger({
            transports: [
                new transports.File({ filename: 'migrations.log' }),
                new transports.Console()
            ]
        });
        this.metrics = this.setupMetrics();
    }

    setupMetrics() {
        const register = new prometheus.Registry();

        return {
            migrationDuration: new prometheus.Histogram({
                name: 'mongodb_migration_duration_seconds',
                he

## Source

Adopted from: antigravity-awesome-skills
