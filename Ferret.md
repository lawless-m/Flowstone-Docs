# Ferret

"A small but eager chatbot" — a [[rust]] web chatbot powered by [[ollama]] for local LLM and the Brave Search API for real-time web queries.

**Repo:** `~/Git/Ferret`
**Themes:** [[rust]], [[ollama]], [[bots]]

A lightweight web server exposes a clean chat UI and a `POST /chat` endpoint that streams replies via server-sent events. Session management with automatic cleanup. The bot calls two tools when it needs to: `brave_search` for web queries and `fetch_page` for retrieving and extracting readable text from URLs. Configurable via env vars: `OLLAMA_URL`, `OLLAMA_MODEL` (default `qwen2.5:7b`), `BRAVE_API_KEY`, `BIND_ADDRESS`, `SESSION_TIMEOUT_MINS`. Fourth bot in the corpus alongside [[Caturiel]], [[Gwen]] (QwenCoder Bot) and [[Robocyril]].
