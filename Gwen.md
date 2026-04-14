# Gwen

An autonomous [[rust]] coding agent — "QwenCoder Bot" — that uses [[Qwen]] 2.5 Coder models via [[ollama]] to automatically implement fixes and features from [[Gogs]] issue tickets, escalating anything too complex back to Claude Code for manual work.

**Repo:** `~/Git/Gwen` (project code lives under `qwencoder-bot/`)
**Themes:** [[rust]], [[ollama]], [[bots]], [[Qwen]], [[Gogs]]

Two-tier design: a 7B model triages each issue ("trivial" / "worth-attempting" / "too-complex"), a 14B model takes on the worth-attempting ones inside a disposable QEMU/KVM snapshot, runs the project's own test command (`cargo test`, `dotnet test`, `pytest`, `shellcheck`), and opens a PR on success or labels the issue `needs-claude-code` on failure. Operates as another profile in Matt's existing `gog` CLI agent ecosystem alongside opus-planning and sonnet-backend agents. Roughly 4,000 lines of Rust landed in a single "feat: implement QwenCoder Bot Rust codebase" commit (Dec 2025) covering assessment, implementation, Gogs client, Ollama client and VM management, on top of seven substantial design documents. **Status:** written but not known to have been exercised end-to-end against real Gogs / Ollama / VMs — a "partially built" project in the sense that the architecture is complete on disk but the runtime loop hasn't been proven in anger.
