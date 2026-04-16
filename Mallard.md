# Mallard

A [[CSharp]] natural-language SQL assistant that converts questions into [[DuckDB]] queries using [[Claude-Api]].

**Repo:** `~/Git/Mallard`

Mallard reads schema metadata from [[Parquet]] files, feeds it to Claude as context, and translates natural-language questions into [[DuckDB]] SQL. Ships as both a CLI and an ASP.NET web service with Windows Authentication. Teaches SQL concepts (CTEs, window functions) as it goes. Exports results to Excel with Power Query .m files for refreshable reports.
