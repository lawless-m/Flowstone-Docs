# Flowstone

A [[Rust]] [[CLITools]] tool that turns a folder of Markdown files into a queryable knowledge graph, backed by [[CozoDB]] and [[Datalog]].

**Repo:** `~/Git/Flowstone`

Flowstone parses `[[WikiLink]]` syntax (and `#tags`) out of plain Markdown, loads notes, links and tags into [[CozoDB]] as relations, and gives you two ways to explore the graph: a Datalog REPL, or an Axum-hosted web UI with a [[D3]] force graph, a tag sidebar, [[FullTextSearch]] via Cozo's [[Tantivy]] FTS, a filesystem watcher that reloads on edit, and a detail panel that renders each note's Markdown body with clickable wiki-links. Notes are the source of truth — the database is purely derived and rebuilt on each run.

The crate is now a small workspace: a `flowstone-core` library holds the schema, parser, and bulk loaders, while the `flowstone` binary is the CLI and server on top. CozoDB comes in via a sibling path dependency on [[Cozordb]] (the fork carrying the [[Redb]] storage backend).

[[Todo]] 

* send updates to documents on the phone just like this
* directed graph for pm - can't do this until I've done that
* e.g. once i have that i can do gannt charts!
