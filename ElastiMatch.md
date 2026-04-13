# ElastiMatch

A [[RocsMiddleware]] diagnostic tool that compares [[elasticsearch]] indexes between production and staging clusters.

**Repo:** `~/Git/RocsMiddleware/ElastiMatch`
**Themes:** [[csharp]], [[dotnet]], [[elasticsearch]]

Scrolls through both clusters using natural keys, reports matches, mismatches, and records only in one side. Supports field filtering and field ignoring. Ad-hoc tool, not scheduled.

## Related

- [[RocsMiddleware]]
- [[ElastiCompare]] — standalone tool with similar purpose but uses parquet intermediary
- [[elasticsearch]]
