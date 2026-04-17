# Charlotte

A [[Rust]] [[TextToSpeech]] library wrapping a local F5-TTS server, with voice cloning and GPU memory management for sharing VRAM with other services.

**Repo:** `~/Git/Charlotte`
**URL:** `https://dw.ramsden-international.com/charlotte/`

Charlotte exposes a simple async Rust API over an HTTP Python server running F5-TTS. It synthesises speech from text and can clone voices from short reference audio clips. The server implements auto-unload-on-idle and OOM retry patterns for sharing the RTX 3090 with [[Ollama]] and other GPU services. Deployed on [[Dw.ramsdenInternational.com]].
