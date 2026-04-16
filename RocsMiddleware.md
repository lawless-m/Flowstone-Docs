# RocsMiddleware

A [[csharp]] monorepo of 16 independent services that synchronise data between [[Sage-X3]], [[ExportMaster]], [[ElasticSearch]], [[Keycloak]], and [[PostgreSQL]].

**Repo:** `~/Git/RocsMiddleware`

RocsMiddleware is the data integration backbone for Ramsden International. All services are .NET 9 console apps running as Windows Scheduled Tasks on RIVSIS02, with PostgreSQL (`x3rocs` on rivsprod01) as the central hub. Data flows in from [[Sage-X3]] and [[ExportMaster]], gets normalised in [[PostgreSQL]] with hash-based change tracking, then fans out to [[ElasticSearch]], [[Keycloak]], and back to [[ExportMaster]]. No orchestrator — each tool runs independently and can be paused, rerun, or debugged in isolation.

