# DoctorDot

A modular [[Python]] chatbot — "HR Policy Chatbot" — for querying PDF document collections using GPU-accelerated semantic embeddings, [[DuckDB]] vector similarity search, and [[Claude-API]] (Claude Sonnet 4) for answer generation.

**Repo:** `~/Git/DoctorDot`

FastAPI backend with a React frontend. Documents are ingested as PDFs, chunked, embedded on the GPU, and stored in DuckDB's vector store (VSS extension). Queries pass through a modular guardrail layer — domain-specific constraint rules — before hitting the retrieval and Claude pipeline. All responses include source citations, so the chatbot is auditable. Shipped with an "HR Policies" guardrail and collection as the first concrete use case, but the guardrail and collection layers are pluggable: the same backend can serve multiple document sets each with its own rules.
