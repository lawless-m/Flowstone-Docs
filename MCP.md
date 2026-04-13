# MCP

Anthropic's Model Context Protocol — a JSON-RPC interface for exposing tools to language models. This corpus has two MCP servers: one wrapping a wargame so LLMs can play the opposing side, one bridging two Claude instances so they can share state.

## Members

- [[BattleForMoscow]] — the `mcp-player` crate wraps the wargame in MCP tools with a narrator that turns game state into descriptive text for the LLM
- [[2claudes1cup]] — `c2c-server`, a Claude-to-Claude MCP bridge with HTTP and stdio transports and SQLite persistence

## Related themes

- [[claude-tooling]]
- [[rust]]
