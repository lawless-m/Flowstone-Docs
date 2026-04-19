# BPQuery

A [[CSharp]] web service for querying business partner permissions and monitoring [[Keycloak]] authentication events in real time.

**Repo:** `~/Git/BPQuery`
**URL:** `https://dw.ramsden-international.com/bpquery/`

BPQuery pulls user and permission data from multiple backends — Sage1000 via SQL Server, [[Keycloak]] user records from MySQL, and authentication event history from [[Parquet]] files via [[DuckDB]] [[ODBC]]. It provides a search interface for business partner lookup by account code, email, or username, plus a live event monitor showing recent logins, logouts, and impersonation activity. Runs as a Windows Service on RIVSPROD02 with Kestrel, reverse-proxied through Apache on [[Dw.RamsdenInternational.Com]].
