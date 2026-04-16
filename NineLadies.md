# NineLadies

A [[Rust]] batch image description CLI using vision language models via [[Ollama]], named after the Nine Ladies stone circle in Derbyshire.

**Repo:** `~/Git/NineLadies`
**URL:** `https://dw.ramsden-international.com/9ladies/`

Reads image paths from stdin, sends each to a vision model (LLaVA, Qwen2.5-VL), and outputs one JSONL object per image to stdout. Prompt files configure system message, temperature, and task (describe, count people, find barcodes). Also ships a web workbench for prompt experimentation. Deployed on [[dw.ramsden-international.com]].
