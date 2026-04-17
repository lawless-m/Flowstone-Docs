# Parquet

Parquet files are a column store file format for analytical data. It has built in compression and indexing and combined with [[DuckDB]] is very fast to query.

Sadly no native access in [[Excel]] although [[PowerBI]] can import data from them.

[[PostgreSQL]] does have a [[ForeignDataWrapper]] for them so they can also be queried there.

They can be created on [[CSharp]] and [[Python]] and plenty of other languages and are an open specification making them excellent containers for many sorts of data. Unlike [[CSV]] the columns are typed Int, Float64 Date DateTime etc. so the string and back probel is eliminated.