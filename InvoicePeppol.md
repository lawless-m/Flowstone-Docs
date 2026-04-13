# InvoicePeppol

A [[RocsMiddleware]] service that generates Peppol BIS Billing 3.0 compliant UBL 2.1 XML invoices.

**Repo:** `~/Git/RocsMiddleware/InvoicePeppol`
**Themes:** [[csharp]], [[dotnet]]

Reads invoice and customer data from PostgreSQL, generates EU Directive 2014/55/EU compliant XML documents for transmission via Descartes middleware to the Peppol network. Outputs to per-customer subdirectories with XSD validation.

## Related

- [[RocsMiddleware]]
- [[InvoiceUploader]] — uploads the same invoices to X3
