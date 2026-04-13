# Claude-Skills

A GitHub template repository containing reusable [[claude-tooling]] skills and slash commands — Matt's spellbook of domain knowledge that can be dropped into any project by clicking "Use this template".

**Repo:** `~/Git/Claude-Skills`
**Themes:** [[claude-tooling]]

Each skill is a Markdown document teaching Claude a specific domain — Databases, Elasticsearch, Rust, SharePoint, Logging, Creating Skills, and roughly twenty more. Commands ship alongside: `/commit`, `/publish`, `/push`. Every project in this corpus that has a `.claude/skills/` folder is drawing from this template, and the Flowstone Docs skill producing these notes lives here too. Maintained internally at Gogs with a post-receive hook that mirrors to GitHub.

## Related

- [[Robocyril]] — uses the template's skills and commands
- [[StinkySpy]] — ships its own skills alongside the shared set
- [[Gwen]] — seeded from this template
- [[TheHand]] — draws from the template for its Claude integration
- [[claude-tooling]]
