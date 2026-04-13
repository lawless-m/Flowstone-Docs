# Qwen

A family of open-weight large language models published by Alibaba's
Tongyi Lab. The useful thing to know for anyone wandering into this
corpus: Qwen is what Matt reaches for whenever he wants a local LLM
that behaves, in place of a hosted Claude or GPT call. The home rig
runs several Qwen 2.5 variants on an NVIDIA 3090 via [[ollama]], with
VRAM doled out across whichever services happen to need inference.

Qwen 2.5 Coder is the specialised coding variant, and any project in
this corpus that mentions a "QwenCoder Bot" is really talking about a
small pipeline around that model.

## Members

- [[Caturiel]] — uses Qwen (via Ollama) to decide what to post to Clacker-News and to write the commentary
- [[Gwen]] — "QwenCoder Bot", a two-tier autonomous coding agent using Qwen 2.5 Coder 7B for issue triage and 14B for implementation, driving fixes to [[Gogs]] tickets

## Related themes

- [[ollama]]
- [[bots]]
- [[rust]]
