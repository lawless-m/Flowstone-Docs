# Anthea

A [[csharp]] price-lookup tool that bypasses a slow multi-service pricing pipeline by querying [[parquet]] files directly via [[DuckDB]].

**Repo:** `~/Git/Anthea`
**URL:** `https://dw.ramsden-international.com/tiny02/anthea.html`
**Themes:** [[csharp]], [[dotnet]], [[DuckDB]], [[parquet]], [[elasticsearch]]

Named after Bruce Forsyth's assistant on *The Price is Right*, Anthea resolves customer-specific product pricing on the fly — eliminating a 90-minute [[elasticsearch]] indexing cycle. It reads [[parquet]] data (products, prices, customers, profiles, exchange rates) from a network share and runs a multi-CTE query through DuckDB to walk the full fallback chain: profile resolution, primary/secondary price lookups, discount application, and currency conversion. Deployed as a self-contained [[dotnet]] 9 CGI executable behind Apache on [[dw.ramsden-international.com]], with a vanilla HTML/JS frontend for ad-hoc lookups and a JSON API for programmatic use.

## Related

- [[csharp]]
- [[dotnet]]
- [[DuckDB]]
- [[parquet]]
- [[elasticsearch]]
- [[dw.ramsden-international.com]]
