# CGI-Sharp

A [[CSharp]] [[CGI]] database query engine that produces [[HTMLDataTable]] — a self-contained executable for serving parameterised SQL results as JSON over HTTP.

**Repo:** `~/Git/CGI-Sharp`

CGI-Sharp takes HTTP query strings, maps them to SQL queries defined in JSON config files, executes them against multiple database backends (SQL Server, [[PostgreSQL]], [[DuckDB]], [[MySQL]], [[Dbisam]]) via [[ODBC]] or native drivers, and returns columnar JSON. The primary output is [[HTMLDataTable]], a trimmed .NET 9 single-file executable deployed to TinyWeb on [[Dw.RamsdenInternational.Com]].

