# 2claudes1cup

A [[Rust]] [[MCP]] server — package name `c2c-server`, repo name a visual pun. Almost certainly a "Claude-to-Claude" bridge: an MCP endpoint that lets two Claude instances share state or pass messages through a common server. Classic spec-then-implementation layout.

**Repo:** `~/Git/2claudes1cup`

`Cargo.toml` names the binary `c2c-server` and pulls in axum (HTTP transport), rusqlite bundled (persistent state), clap, tokio, tracing and serde — a standard MCP-server stack. The `src/` layout (`http.rs`, `mcp.rs`, `stdio.rs`, `db.rs`, `config.rs`, `main.rs`) confirms two MCP transports (HTTP + stdio), SQLite persistence, and config loading. Design docs live in `c2c-design/` as `C2C_DESIGN.md` and `CONTENTS.md`, extracted from `c2c-design.zip`. **Status:** code and design are both present, README is missing; this is a working build, not a placeholder.
