# Anthea

A [[CSharp]] price-lookup tool that bypasses a slow multi-service pricing pipeline by querying [[Parquet]] files directly via [[DuckDB]].

**Repo:** `~/Git/Anthea`
**URL:** `https://dw.ramsden-international.com/tiny02/anthea.html`

Named after Bruce Forsyth's assistant on *The Generation Game* and later wife, Anthea resolves customer-specific product pricing on the fly — eliminating an [[Elasticsearch]] query and indexing cycle. It reads [[Parquet]] data (products, prices, customers, profiles, exchange rates) from a network share and runs an SQL query through [[DuckDB]] to walk the full fallback chain: profile resolution, primary/secondary price lookups, discount application, and currency conversion. Deployed as a self-contained [[Dotnet]] 9 [[CGI]] executable behind Apache on [[Dw.ramsden-International.com]], with a vanilla HTML/JS frontend for ad-hoc lookups and a JSON API for programmatic use.

