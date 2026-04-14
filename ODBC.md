# ODBC

Open Database Connectivity — the primary access method for reaching [[DBISAM]], [[DuckDB]], and SQL Server databases from .NET services in this corpus. Most connections go through Windows ODBC DSNs configured on the host machines.

## Members

- [[CGI-Sharp]] — uses ODBC to query multiple database backends
- [[HTMLDataTable]] — the CGI executable connecting via ODBC DSNs
- [[ODBCQuery]] — generic CLI tool for running SQL against any ODBC source
- [[FakeODBC]] — a mock ODBC driver returning static CSV data
- [[CustomerIndexer]] — reads ExportMaster via ODBC
- [[EMUpdater]] — reads PostgreSQL via ODBC
- [[InvoiceExtractor]] — reads ExportMaster via ODBC
- [[X3CustomerPull]] — reads X3 SQL Server via ODBC
- [[PriceDiscountExtractor]] — reads X3 SQL Server via ODBC
- [[PriceExtractor]] — reads parquet via DuckDB ODBC
- [[ParquetToPostgres]] — reads parquet via DuckDB ODBC
- [[Plaster1-WorkInvoice]] — reads ExportMaster via ODBC
- [[JordanPrice]] — reads ExportMaster via ODBC
- [[BPQuery]] — reads Keycloak events via DuckDB ODBC

## Related themes

- [[DBISAM]] — ExportMaster's database, accessed via ODBC
- [[DuckDB]] — parquet queries routed through DuckDB's ODBC driver
- [[ExportMaster]] — the main DBISAM application
- [[csharp]] — all ODBC consumers are .NET
