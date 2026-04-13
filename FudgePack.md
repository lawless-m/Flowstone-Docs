# FudgePack

A [[rust]] food packaging verification system that extracts structured data from photos of packaging using vision AI.

**Repo:** `~/Git/FudgePack`
**Themes:** [[rust]], [[claude-api]], [[ollama]]

FudgePack photographs food packaging and uses Claude Haiku or local [[ollama]] vision models (Qwen 2.5 VL) to extract ingredients, allergens, and product details into structured JSON. Compares against known ingredient records to catch supply chain changes that could trigger rejections or bans. Ships as an Axum web server with drag-and-drop UI, plus a CLI for batch directory processing with barcode scanning and Excel/CSV output.

## Related

- [[rust]]
- [[claude-api]]
- [[ollama]]
