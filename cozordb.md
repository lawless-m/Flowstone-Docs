# cozordb

Matt's [[rust]]-only fork of [[CozoDB]] published as `lawless-m/cozo-redb`. Strips the upstream multi-backend story down to a single persistent backend ([[redb]]) plus an in-memory backend, removes the Python/Node/Java/Swift/C bindings, and targets Rust embedders exclusively. [[Flowstone]] is the primary in-corpus consumer.

**Repo:** `~/Git/cozordb/cozo`

The fork's two interesting moves beyond "remove things": (1) full-text search is reimplemented as a thin bridge to [[tantivy]], replacing the deleted upstream FTS engine; (2) `cozo-lib-wasm` is a working `wasm-pack` build that exposes a `CozoDb` JS class over the in-memory backend, with full-text search included via an in-RAM tantivy index. The native default uses an on-disk tantivy directory next to the redb file (`fts-mmap` feature); the [[WASM]] build uses RAM mode (`fts` feature) and rebuilds the index on every database open. Compiling the [[WASM]] target needs a wasm-capable clang because `tantivy-sstable` pulls in `zstd-sys`'s C shim — `cozo-lib-wasm/build.sh` defaults to `clang-19` and bails early if it's missing.
