# tantivy

The Rust full-text search library by Quickwit — a Lucene analogue, with `QueryParser`, tokenizers, schemas, and an inverted index. Used in this corpus as the engine behind CozoDB's `~rel:ft{query: "..."}` syntax.

## Members

- [[cozordb]] — bridges CozoDB to tantivy in `cozo-core/src/fts/mod.rs`, with both on-disk (`fts-mmap`) and in-RAM (`fts`) modes
- [[Flowstone]] — consumes the bridge transitively, via cozordb's FTS, for its web UI search

## Related themes

- [[full-text-search]]
- [[rust]]
- [[CozoDB]]
