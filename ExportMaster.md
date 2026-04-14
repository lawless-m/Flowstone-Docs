# ExportMaster

The company's order processing system — handles quotes, orders, invoices, shipments, and product data. Backed by a [[DBISAM]] database, accessed via ODBC or its COM DLL interface (ECNICI.E3CustomerInterface).

## Members

- [[RocsMiddleware]] — the integration backbone; multiple children sync data to/from EM
- [[CustomerIndexer]] — indexes EM customer profiles into Elasticsearch
- [[EMUpdater]] — pushes customer/discount data back into EM via COM DLL
- [[InvoiceExtractor]] — pulls invoices from EM into PostgreSQL
- [[CreditStatusCGI]] — serves credit data for EM consumption via FakeODBC
- [[JordanPrice]] — part of the pricing pipeline originating from EM data
- [[MasterBlaster]] — automates EM's UI over RDP using Claude vision
- [[EM-Document-Scripts]] — VBScript print templates for EM's document system
- [[CGI-Sharp]] — queries EM's DBISAM database via HTMLDataTable
- [[HTMLDataTable]] — the CGI executable that queries EM
- [[Plaster1-WorkInvoice]] — pulls repro shipment data from EM
- [[PowerQueries]] — Power Query modules querying EM via ODBC
- [[Gravedigger]] — VSS-based backup of EM's DBISAM files

## Related themes

- [[DBISAM]] — the database engine behind ExportMaster
- [[ODBC]] — primary access method for reading EM data
- [[csharp]] — most EM integrations are .NET
- [[dw.ramsden-international.com]] — hosts CGI services that query EM
