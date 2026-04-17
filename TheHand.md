# TheHand

A [[Rust]] voice-activated transcription tool that continuously listens, auto-records when you start speaking, transcribes with [[Whisper]] when you stop, and types the result straight into whatever window has focus.

**Repo:** `~/Git/TheHand`

Built for Linux. Listens on ALSA, uses silence detection to bracket utterances, and hands the audio to a GPU-accelerated whisper.cpp server (with a CLI fallback for CPU-only setups). Output is synthesised keystrokes via libXtst, so any focused application receives the transcript as if typed. Also handles voice commands — bind a phrase to a keybind or a shell command. Ships with a VU meter, a transcription history, i3blocks integration, and a mute mode. Original motivation: feeding voice prompts into Claude Code without touching the keyboard.
