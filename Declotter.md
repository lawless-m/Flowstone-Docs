# Declotter

A [[CSharp]] product description compressor that squeezes long product names into a 40-character database limit using AI-assisted abbreviation.

**Repo:** `~/Git/Declotter`
**URL:** `https://dw.ramsden-international.com/tiny02/cgi-bin/Declotter-Web-CGI.exe`

Declotter has three implementations: a rule-based original, a local [[ollama]]-powered version using Qwen, and a [[claude-api]] version using Anthropic's tiered model selection (Haiku first, escalating to Sonnet/Opus when needed). All three learn compression patterns from 1000+ existing manually-compressed descriptions via few-shot examples stored in [[Parquet]]. Deployed as a CGI executable on [[dw.ramsden-international.com]] for integration with Excel/VBA workflows.
