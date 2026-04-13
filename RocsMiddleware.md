# RocsMiddleware

A [[csharp]] monorepo of 16 independent services that synchronise data between [[sage-x3]], [[ExportMaster]], [[elasticsearch]], [[Keycloak]], and PostgreSQL.

**Repo:** `~/Git/RocsMiddleware`
**Themes:** [[csharp]], [[dotnet]], [[sage-x3]], [[ExportMaster]], [[elasticsearch]], [[Keycloak]], [[ODBC]], [[parquet]], [[DBISAM]]

RocsMiddleware is the data integration backbone for Ramsden International. All services are .NET 9 console apps running as Windows Scheduled Tasks on RIVSIS02, with PostgreSQL (`x3rocs` on rivsprod01) as the central hub. Data flows in from [[sage-x3]] and [[ExportMaster]], gets normalised in PostgreSQL with hash-based change tracking, then fans out to [[elasticsearch]], [[Keycloak]], and back to ExportMaster. No orchestrator — each tool runs independently and can be paused, rerun, or debugged in isolation.

## Children

- [[DashboardCGI]] — real-time monitoring dashboard for service stats
- [[InvoiceUploader]] — pushes invoices from PostgreSQL to X3 REST API
- [[CustomerIndexer]] — syncs customer data to Elasticsearch
- [[InvoicePeppol]] — generates Peppol BIS 3.0 UBL XML invoices
- [[KeycloakUpdater]] — syncs contacts to Keycloak user management
- [[EMUpdater]] — pushes customer/discount data back to ExportMaster via COM DLL
- [[CreditStatusCGI]] — CGI endpoint exporting credit status as CSV
- [[CreditStatus]] — fetches credit limits from X3 REST API
- [[PriceExtractor]] — loads pricing from parquet files into PostgreSQL
- [[ElastiMatch]] — diagnostic comparing prod vs staging Elasticsearch indexes
- [[X3CustomerPull]] — core feeder pulling customers from X3 into PostgreSQL
- [[InvoiceExtractor]] — extracts invoices from ExportMaster into PostgreSQL
- [[DeleteRocsQuote]] — manual tool for removing unordered quotes from Elasticsearch
- [[PriceDiscountUploader]] — pushes price discount changes to Elasticsearch
- [[PriceDiscountExtractor]] — pulls price discounts directly from X3 SQL Server
- [[InvalidQuoteIdFinder]] — diagnostic for detecting broken quote references

## Related

- [[csharp]]
- [[dotnet]]
- [[sage-x3]]
- [[ExportMaster]]
- [[elasticsearch]]
- [[Keycloak]]
- [[ODBC]]
- [[parquet]]
- [[DBISAM]]
- [[dw.ramsden-international.com]]
