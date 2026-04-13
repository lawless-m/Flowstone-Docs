# Gravedigger

A [[csharp]] [[DBISAM]] replication tool that creates non-intrusive backups via Windows Volume Shadow Copy (VSS).

**Repo:** `~/Git/Gravedigger`
**Themes:** [[csharp]], [[dotnet]], [[DBISAM]]

Gravedigger extracts [[DBISAM]] database files from VSS shadow copies to produce consistent replicas without stopping or locking the running database. Supports generation management (auto-cleanup of old replicas), file validation, retry logic, and scheduled execution via Windows Task Scheduler. Deployed as a self-contained .NET 8 single-file executable.

## Related

- [[csharp]]
- [[dotnet]]
- [[DBISAM]]
