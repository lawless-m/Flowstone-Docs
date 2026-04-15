# Biscuits

A [[csharp]] desktop tool for inspecting [[PowerBI]] files — connects to a running PBI Desktop instance and identifies unused tables, measures, and columns.

**Repo:** `~/Git/Biscuits`

Biscuits (PBI Inspector) replaces the commercial "Measure Killer" tool. It connects to the local Analysis Services instance that Power BI Desktop spins up, reads the Tabular Object Model, parses DAX dependencies, and cross-references with the report layout extracted from the .pbix ZIP. The result is three views — Report, Model, and Orphans — showing what's used, what's indirectly referenced, and what's dead weight. Built as a self-contained .NET 9 executable with a React/[[Typescript]] frontend served via Kestrel on localhost.
