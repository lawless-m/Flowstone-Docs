# Ztil

A [[rust]] emulator for the **Research Machines 380Z** — a British 8-bit [[Z80]] microcomputer from 1977–80 that was widely used in UK schools before the BBC Micro landed. Cargo workspace with a core emulator, a native binary runner, a web server front end, and a [[wasm]] target so the machine can run inside a browser tab.

**Repo:** `~/Git/Ztil`

Workspace members: `rm380z-core` (the emulator engine), `rm380z` (the native runner binary), `rm380z-server` (a web server front end), `rm380z-wasm` (the WebAssembly build), and a `z80/` crate that almost certainly holds the CPU emulation itself. `disks/` holds disk images for software to load. Documentation lives in `zip-til-docs/`, extracted from a zip — the spec-then-implementation pattern again. A `deploy/` folder hints at a hosted version, and a tiny `run` script sits at the root as a convenience launcher. Retrocomputing labour of love rather than anything practical.
