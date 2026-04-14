# X3CustomerPull

A [[RocsMiddleware]] core feeder service that pulls customer data from [[sage-x3]] into PostgreSQL.

**Repo:** `~/Git/RocsMiddleware/X3CustomerPull`
**Themes:** [[csharp]], [[dotnet]], [[sage-x3]], [[ODBC]]

Queries the X3 REST API for recently updated customers (2-hour window with DST buffer), fetches EORI numbers via direct X3 SQL Server [[ODBC]], and syncs to PostgreSQL `x3.customer` with hash-based change detection. Supports incremental and full sync modes.
