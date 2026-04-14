# CreditStatus

A [[RocsMiddleware]] service that fetches customer credit limits and unpaid amounts from the [[sage-x3]] REST API.

**Repo:** `~/Git/RocsMiddleware/CreditStatus`
**Themes:** [[csharp]], [[dotnet]], [[sage-x3]]

Calls the X3 Credit Status endpoint for individual or all customers and stores results in PostgreSQL `x3.credit_status` with timestamp tracking.
