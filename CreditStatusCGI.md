# CreditStatusCGI

A [[RocsMiddleware]] CGI endpoint that exports customer credit status as CSV for [[ExportMaster]] consumption.

**Repo:** `~/Git/RocsMiddleware/CreditStatusCGI`
**Themes:** [[csharp]], [[dotnet]], [[ExportMaster]]

Queries PostgreSQL `x3.credit_status` and returns CSV (customer, unpaid amount, credit limit). ExportMaster reads this via [[FakeODBC]], which ignores SQL and returns the CGI response instead.

## Related

- [[RocsMiddleware]]
- [[CreditStatus]] — upstream: fetches credit data from X3
- [[FakeODBC]] — the mock ODBC driver that serves this data to ExportMaster
- [[ExportMaster]]
