# elasticsearch

Elasticsearch 5.2 search clusters — production and staging — used for product, customer, pricing, and quote search across the ROCS platform.

Two clusters:
- **Production:** `rocs-production-es.ramsden-international.com`
- **Staging:** `rocs-stage-es.ramsden-international.com`

Key indexes: `price_discount`, `customers`, `quotes`, `shipments`, `orders`.

## Members

- [[Anthea]] — replaces a slow ES indexing cycle for pricing
- [[CustomerIndexer]] — syncs customer data into ES
- [[DeleteRocsQuote]] — removes unordered quotes/shipments from ES
- [[ElastiCompare]] — compares prod vs staging via parquet intermediary
- [[ElastiMatch]] — compares prod vs staging by scrolling both clusters
- [[ESIndexDownloader]] — downloads entire indexes to JSON
- [[InvalidQuoteIdFinder]] — detects broken quote references in ES
- [[JordanPrice]] — bulk-indexes price discounts with zero-downtime alias swaps
- [[PgTripEs]] — syncs PostgreSQL price_discount changes to ES
- [[PriceDiscountUploader]] — pushes price discount changes to ES
- [[PriceExtractor]] — queries ES for current pricing period
- [[RocsMiddleware]] — parent monorepo; most ES interaction flows through its children

## Related themes

- [[parquet]] — often used as intermediate format when downloading from ES
- [[DuckDB]] — queries parquet dumps of ES data
- [[csharp]] — all ES clients in this corpus are .NET
- [[sage-x3]] — upstream data source for much of what lands in ES
- [[ExportMaster]] — other upstream data source
