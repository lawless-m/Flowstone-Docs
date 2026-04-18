# Fayregrind

A [[CSharp]] CLI tool that finds products missing from the `niingred` ingredient table in [[ExportMaster]] and inserts them.

**Repo:** `~/Git/Fayregrind`
**Binary:** `Y:\CSharpDLLs\Fayregrind\Fayregrind.exe`

Fayregrind connects to [[ExportMaster]] via [[ODBC]] and LEFT JOINs the `product` table against `niingred` to find products with valid barcodes (8 or 13 digits) that have no English ingredient record. It builds a description from `UF_UKLDESC` or `DESC3`/`DESC4`/`DESC5` and inserts one row per gap. Supports a `--simulate` flag to preview INSERT statements without writing to [[Dbisam]]. Published as a self-contained single-file exe.
