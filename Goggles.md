# Goggles

A [[rust]] [[cli-tools]] implementation of a [[Gogs]] command-line client — the `gog` CLI that several projects in this corpus reference, notably [[Gwen]]'s QwenCoder Bot (which operates as another `gog` profile alongside opus-planning and sonnet-backend agents). Name is a pun on "Gogs CLI".

**Repo:** `~/Git/Goggles`
**Themes:** [[rust]], [[cli-tools]], [[Gogs]]

Spec-then-implementation layout: `gogs-cli-spec/` holds the design documents (extracted from `gogs-cli-specification.zip`), and `gogs-cli/` holds the Rust implementation. This is the tool that makes Matt's multi-agent workflow possible — the way bots pick up issue tickets, comment on them as named profiles, and coordinate through Gogs as a shared workspace. **Status:** the repo root still carries [[Claude-Skills]] template artifacts; a detemplate pass is pending. The real work lives under the two subfolders.
