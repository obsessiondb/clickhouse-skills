# ClickHouse Skills for Claude Code

Build ClickHouse tables with sub-second queries, 10x compression, and zero full table scans.

## Installation

```bash
npx skills add https://github.com/obsessiondb/clickhouse-skills
```

## Available Skills

| Skill                             | Rules | Trigger                                                       |
| --------------------------------- | ----- | ------------------------------------------------------------- |
| **clickhouse-schema-design**      | 15+   | Creating/modifying tables, ORDER BY, PARTITION BY, TTL        |
| **clickhouse-query-optimization** | 20+   | Writing/debugging queries, slow queries, JOINs, memory errors |
| **clickhouse-materialized-views** | 10+   | Creating MVs, real-time aggregation, pre-aggregation          |

## How Skills Work

Skills load automatically when relevant tasks are detected:

- Mention "CREATE TABLE" or "schema" → loads **schema-design**
- Mention "slow query", "JOIN", or "optimize" → loads **query-optimization**
- Mention "materialized view" or "MV" → loads **materialized-views**

## Skill Structure

Each skill contains a `SKILL.md` file with:

- **Goals** - Measurable outcomes (e.g., "10x compression")
- **Critical Rules** - Prioritized as CRITICAL, HIGH, MEDIUM
- **Patterns** - Good vs Bad code examples
- **Troubleshooting** - Common problems and solutions

## Contributing

Contributions welcome! See [AGENTS.md](AGENTS.md) for skill authoring guidelines.

## License

MIT + Commons Clause (free to use, not for resale)

## Sponsor

Sponsored by [ObsessionDB](https://obsessiondb.com)
