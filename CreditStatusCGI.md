# CreditStatusCGI

A [[RocsMiddleware]] CGI endpoint that exports customer credit status as CSV for [[ExportMaster]] consumption.

**Repo:** `~/Git/RocsMiddleware/CreditStatusCGI`

Queries PostgreSQL `x3.credit_status` and returns CSV (customer, unpaid amount, credit limit). ExportMaster reads this via [[FakeOdbc]], which ignores SQL and returns the CGI response instead.
