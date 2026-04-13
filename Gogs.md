# Gogs

The self-hosted Git service Matt runs at `dw.ramsden-international.com`, which doubles as the coordination layer for his multi-agent workflow. Bots pick up issues tagged with specific labels (e.g. `qwen-candidate`), comment as named profiles (`opus-planning`, `sonnet-backend`, `qwen-coder`, `qwen-assessor`), open pull requests for human review on success, and escalate with a `needs-claude-code` label on failure.

## Members

- [[Goggles]] — the `gog` Rust CLI, the tool every agent profile runs through
- [[Gwen]] — QwenCoder Bot, operates as a `gog` profile alongside the others

## Related themes

- [[claude-tooling]]
- [[bots]]
- [[cli-tools]]
