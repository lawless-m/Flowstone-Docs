# Gogs

The self-hosted Git service Matt runs at [[Dw.ramsdenInternational.com]], which doubles as the coordination layer for his multi-agent workflow. Bots pick up issues tagged with specific labels (e.g. `qwen-candidate`), comment as named profiles (`opus-planning`, `sonnet-backend`, `qwen-coder`, `qwen-assessor`), open pull requests for human review on success, and escalate with a `needs-claude-code` label on failure.
