# DashboardCGI

A [[RocsMiddleware]] CGI service that provides a real-time monitoring dashboard for invoice and customer sync statistics.

**Repo:** `~/Git/RocsMiddleware/DashboardCGI`
**Themes:** [[csharp]], [[dotnet]]

Queries PostgreSQL for invoice and customer counts (new, updated, failed) and serves them as JSON via TinyWeb CGI endpoints. Auto-refreshes every 30 seconds.
