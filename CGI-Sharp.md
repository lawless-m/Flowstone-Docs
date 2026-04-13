# CGI-Sharp

A [[csharp]] CGI database query engine that produces [[HTMLDataTable]] — a self-contained executable for serving parameterised SQL results as JSON over HTTP.

**Repo:** `~/Git/CGI-Sharp`
**Themes:** [[csharp]], [[dotnet]], [[DBISAM]], [[DuckDB]], [[ODBC]]

CGI-Sharp takes HTTP query strings, maps them to SQL queries defined in JSON config files, executes them against multiple database backends (SQL Server, PostgreSQL, [[DuckDB]], MySQL, [[DBISAM]]) via [[ODBC]] or native drivers, and returns columnar JSON. The primary output is [[HTMLDataTable]], a trimmed .NET 9 single-file executable deployed to TinyWeb on [[dw.ramsden-international.com]].

## Related

- [[HTMLDataTable]] — the executable this project produces
- [[Dingo]] — uses HTMLDataTable for shipment data
- [[Anthea]] — sibling app on the same TinyWeb server
- [[csharp]]
- [[dotnet]]
- [[DuckDB]]
- [[DBISAM]]
- [[ODBC]]
- [[dw.ramsden-international.com]]
