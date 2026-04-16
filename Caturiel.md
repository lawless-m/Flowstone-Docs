# Caturiel

A [[Rust]] bot that monitors Reddit for anti-AI sentiment and posts Uriel-voiced commentary to [[Clacker-News]].

**Repo:** `~/Git/Caturiel`

Caturiel uses [[Ollama]] (Qwen models) to pick what to post and to write the commentary. It persists seen-content state in [[SQLite]] and notifies via ntfy.sh. The personality is deliberately terse and deadpan — it points out irony without cruelty.
