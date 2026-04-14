# FacRepl

A [[rust]] + Prolog tool — "Factorio Constraint Builder" — for generating and placing Factorio factory layouts via a custom DSL, an interactive REPL, an RCON bridge to the running game, and a Scryer Prolog CLP(Z) constraint solver that can synthesise layouts from high-level production goals.

**Repo:** `~/Git/FacRepl`

Five components stacked together. A Factorio Lua mod that listens on RCON and actually places, queries and removes entities in-game. A Rust RCON bridge holding the TCP connection. A Rust DSL parser and executor that handles entity placement, undo/redo, state snapshots, and area operations (`what-at`, `can-place`, `area`, `clear`). An interactive REPL on top. And — the interesting bit — a Scryer Prolog constraint solver using CLP(Z) integer finite-domain constraints that synthesises placements from production goals, so you can describe "I want 60 green circuits per second" and have it plan belts, inserters, assemblers and power. Covers belts (yellow/red/blue), underground belts, splitters with filters and priorities, all inserter types, assemblers 1/2/3, power poles, pipes, pumps, and storage tanks.
