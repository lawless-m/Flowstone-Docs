# glossy

A collection of [[Rust]] and [[Python]] tools for parsing, classifying, and auditing food product ingredient lists using [[Ollama]].

**Repo:** `~/Git/glossy`
**URL:** `https://dw.ramsden-international.com/glossy/`

The main tool is an ingredient parser that takes messy ingredient strings from Parquet, sends them to Qwen via Ollama, and stores structured hierarchical JSON (with sub-ingredients and percentages) into [[DuckDB]]. Also includes ingredient classifiers, normalisers, a CGI audit interface, and order/product audit scripts. Related to [[FudgePack]] — glossy parses the canonical ingredient database, FudgePack verifies what's on the physical packaging. Deployed on [[Dw.ramsden-International.com]].
