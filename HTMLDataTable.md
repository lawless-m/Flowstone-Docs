# HTMLDataTable

The CGI executable produced by [[CGI-Sharp]] — takes HTTP query strings, runs parameterised SQL from JSON config files, and returns columnar JSON.

**Repo:** `~/Git/CGI-Sharp`
**URL:** `https://dw.ramsden-international.com/tiny02/cgi-bin/HTMLDataTable.exe`
**Themes:** [[csharp]], [[dotnet]], [[ODBC]], [[DuckDB]], [[DBISAM]], [[ExportMaster]]

HTMLDataTable is invoked via `?json=<name>&param1=value1`. It loads a JSON config from `C:\RI Services\JsonParams\cgi\<name>.json`, connects to the specified database (PostgreSQL, MySQL, [[DuckDB]], [[DBISAM]]/[[ExportMaster]], or any [[ODBC]] DSN), runs the SQL with parameter substitution, and returns results as columnar JSON.

## JSON config format

Each config file is an array of query definitions:

```json
[
  {
    "dsn": "DW",
    "sql": ["SELECT col FROM table WHERE key = @param"],
    "paramcount": 1
  }
]
```

Key fields: `dsn` (connection target), `sql` (inline array) or `sqlfile` (external .sql filename without extension), `paramcount` (expected parameters), plus optional `host`/`port`/`database`/`user`/`password` for MySQL, `credentials` (path to creds JSON), and `useWindowsAuth`.

## Output format

```json
{
  "headers": ["col1", "col2"],
  "types": ["string", "number"],
  "rows": [["val", 42], ["val2", 17]]
}
```

Types map from .NET: `string`, `datetime` (ISO 8601), `integer`, `number`, `boolean`, `object`. Nulls are JSON `null`. [[PowerQueries]] contains Power Query M modules for consuming this format in Power BI and Excel.
