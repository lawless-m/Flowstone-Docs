# Charlotte

A [[rust]] text-to-speech library wrapping a local F5-TTS server, with voice cloning and GPU memory management for sharing VRAM with other services.

**Repo:** `~/Git/Charlotte`
**URL:** `https://dw.ramsden-international.com/charlotte/`

Charlotte exposes a simple async Rust API over an HTTP Python server running F5-TTS. It synthesises speech from text and can clone voices from short reference audio clips. The server implements auto-unload-on-idle and OOM retry patterns for sharing the RTX 3090 with [[ollama]] and other GPU services. Deployed on [[dw.ramsden-international.com]].
