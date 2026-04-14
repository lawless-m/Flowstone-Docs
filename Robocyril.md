# Robocyril

A blog system where Claude Code writes posts in the voice of Cyril — a grumpy-but-pragmatic maintenance manager. The punchline: Cyril is vocally anti-vibe-coding while being entirely vibe-coded into existence.

**Repo:** `~/Git/Robocyril`
**Themes:** [[rust]], [[claude-tooling]], [[SQLite]]

Backend is [[rust]] CGI binaries behind nginx talking to [[SQLite]] — 1990s simplicity. Frontend is a Svelte SPA — 2020s overkill. The architectural equivalent of a mullet. You type `/blog <topic>` in Claude Code, Claude drafts a post in Cyril's voice, a POST to the API creates the entry, and visitors see a gloriously over-engineered SPA serving content from CGI binaries. Ships with `/blog`, `/commit` and `/push` slash commands and a small set of Claude Code skills drawn from [[Claude-Skills]].
