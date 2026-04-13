# Dressage

A [[csharp]] address normalisation service that parses freeform address text into structured JSON using [[claude-api]].

**Repo:** `~/Git/Dressage`
**URL:** `https://dw.ramsden-international.com/tiny02/cgi-bin/Dressage.Cgi.exe`
**Themes:** [[csharp]], [[dotnet]], [[claude-api]]

Dressage takes messy, unformatted address strings and returns clean, component-based address objects with confidence scores. It calls Claude Haiku for the parsing intelligence — cheap enough at ~$0.10 per 1000 addresses. Ships as two executables: a CGI endpoint on [[dw.ramsden-international.com]] for live requests and a batch tool for bulk file processing. Sends 20 addresses per API call for cost efficiency, with retry logic and graceful degradation on failures.

## Related

- [[Declotter]] — sibling CGI tool using similar AI-assisted text processing
- [[csharp]]
- [[dotnet]]
- [[claude-api]]
- [[dw.ramsden-international.com]]
