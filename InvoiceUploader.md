# InvoiceUploader

A [[RocsMiddleware]] service that uploads invoices from PostgreSQL to [[sage-x3]] via its REST API.

**Repo:** `~/Git/RocsMiddleware/InvoiceUploader`

Reads unprocessed invoices from PostgreSQL, generates JSON payloads via a stored procedure, posts to the X3 Customer BP Invoice endpoint with a 250ms delay between calls, and records X3 document numbers or failures back to the database.
