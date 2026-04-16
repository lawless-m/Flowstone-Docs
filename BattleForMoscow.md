# BattleForMoscow

A web implementation of Frank Chadwick's 1986 board wargame *Battle for Moscow* (Operation Typhoon, October–December 1941), with a full [[Rust]] Axum backend, an SVG hex map, and — the interesting twist — a separate [[MCP]] player crate that lets LLMs take the opposing side.

**Repo:** `~/Git/BattleForMoscow`

A Cargo workspace with two crates. `backend/` is the game engine: hex geometry (axial coordinates), map data, unit state, turn/phase management, zone-of-control calculations, movement validation and pathfinding, a combat results table implementation, replacement and retreat mechanics — all exposed as a REST API. `mcp-player/` is an MCP server that wraps the game in LLM-friendly tools: a `narrator.rs` that turns game state into descriptive text, a JSON-RPC server implementing the Model Context Protocol, phase-specific prompts, and an alternative text-mode REPL for humans who want terminal-only play. 39 units are parsed from `data/units.json`; map data was still a placeholder at last touch.
