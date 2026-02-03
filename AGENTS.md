# Agent Guidelines for ClickHouse Skills

## Repository Purpose

A collection of ClickHouse-focused skills for Claude Code that help developers design optimal schemas, write performant queries, and implement materialized views.

## Directory Structure

```
skills/
  clickhouse-schema-design/
    SKILL.md           # Agent instructions
  clickhouse-query-optimization/
    SKILL.md
  clickhouse-materialized-views/
    SKILL.md
```

- Skills use `kebab-case` naming in `skills/` directory
- Each skill requires a `SKILL.md` file with YAML frontmatter

## SKILL.md Template

```yaml
---
name: skill-name
description: "Rule count + trigger phrase + measurable outcome"
---
```

```markdown
# Skill Title

**ALWAYS LOAD** or **Load when** [trigger conditions]

## Goals

- Measurable outcome 1 (e.g., "Sub-second queries on billion rows")
- Measurable outcome 2

## Reference Documentation

- [Link 1](url)
- [Link 2](url)

**Search terms:** keyword1, keyword2, keyword3

## Critical Rules

### [CRITICAL]

1. **Rule statement.** Brief explanation.

### [HIGH]

2. **Rule statement.** Brief explanation.

### [MEDIUM]

3. **Rule statement.** Brief explanation.

## Patterns

### Pattern Name

```sql
-- BAD: Why this is wrong
SELECT ...

-- GOOD: Why this is right
SELECT ...
```

## Troubleshooting

### Problem Name

**Problem:** Description of symptoms

**Diagnose:**

```sql
-- Query to identify the issue
```

**Solutions:**

| Cause | Fix |
|-------|-----|
| Cause 1 | Solution 1 |
```

## Best Practices

- Keep SKILL.md under 700 lines
- Use imperative voice ("Do X" not "You should consider X")
- Include Good vs Bad code comparisons
- Add verification queries where applicable
- Prioritize rules by impact: CRITICAL > HIGH > MEDIUM
