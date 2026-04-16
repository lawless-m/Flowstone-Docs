# Ok2BeMail

A [[Rust]] email classifier that fetches corporate mail from Office 365 via Microsoft Graph, classifies it locally with [[Ollama]], and notifies on important items.

**Repo:** `~/Git/Ok2BeMail`

Pulls email from [[Microsoft-Teams]] / Office 365, stores locally in SQLite, and uses Qwen via Ollama for few-shot classification into categories (HR, system alerts, external, junk) with importance scoring. Learns from user corrections through retrieval-augmented few-shot examples using embeddings. All analysis stays on-premises — no email content leaves the local network.
