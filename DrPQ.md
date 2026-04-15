# DrPQ

A [[csharp]] CLI tool for searching across all columns in a folder of [[Parquet]] files.

**Repo:** `~/Git/DrPQ`

DrPQ takes a folder path and a search value, then scans every column in every row group across all Parquet files, reporting matches with file, column, and row group. Case-insensitive substring matching with early termination per column. Useful when you know a value exists somewhere in a large Parquet dataset but not which file or column it's in.
