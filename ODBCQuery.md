# ODBCQuery

A [[csharp]] CLI tool for running SQL queries against any [[ODBC]] data source and outputting results as formatted tables.

**Repo:** `~/Git/ODBCQuery`

ODBCQuery takes a JSON config (DSN + timeout) and SQL via command line or file, executes it over [[ODBC]], and prints results. Supports multiple semicolon-separated statements and both query and non-query commands. Default config targets [[DuckDB]].
