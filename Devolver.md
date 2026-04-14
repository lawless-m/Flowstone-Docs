# Devolver

A [[rust]] [[cli-tools]] utility — the binary is called `devlog` — that captures Claude Code conversations for later reference by ingesting session JSONL files and writing human-readable per-session JSON records into a `.devlog/` folder next to the code being worked on. Context compression loses the "how did we build this" narrative; Devolver puts it back.

**Repo:** `~/Git/Devolver` (repo name and tool name differ: repo is Devolver, binary is `devlog`)
**Themes:** [[rust]], [[cli-tools]], [[claude-tooling]]

Filters the raw JSONL to user prompts, assistant text responses and tool summaries, then enriches each session with git metadata (remote, branch, commit). Output files are named `YYYY-MM-DD-HHMMSS-<session_id_short>.json` and live in `.devlog/` inside each project. Wired up through Claude Code's `PreCompact` and `SessionEnd` hooks via `.claude/settings.json`, so every project accumulates its own conversation history automatically. Most other repos in this corpus already carry a `.devlog/` folder — this is the tool that writes them. (It's also how the "Versatile over Ethernet" hallucination showed up in [[VoE]]'s devlog files — a hallucinated cover story, preserved for posterity.)
