# OneCuriousRabbit

A [[Rust]] invoice OCR system that extracts structured data from PDF invoices using multimodal vision models running locally on GPU.

**Repo:** `~/Git/OneCuriousRabbit`
**URL:** `https://dw.ramsden-international.com/rabbit/`

Converts PDFs to images and sends them to a local Qwen2-VL inference server for extraction of headers, line items, and totals with confidence scoring. Outputs JSON, CSV, and Excel. Batch processing with retry logic, automatic archiving, and a drag-and-drop web UI. Shares GPU VRAM with [[Ollama]] and [[Charlotte]] via OOM retry and request-unload signalling. Deployed on [[dw.ramsden-international.com]].
