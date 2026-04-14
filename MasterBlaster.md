# MasterBlaster

A [[csharp]] desktop automation engine that drives legacy Windows apps over RDP using Claude vision.

**Repo:** `~/Git/MasterBlaster`
**Themes:** [[csharp]], [[dotnet]], [[claude-api]], [[ExportMaster]]

MasterBlaster captures screenshots from an RDP session, sends them to [[claude-api]] for visual analysis, and executes mouse/keyboard actions based on what Claude identifies on screen. Has a custom declarative language (MBL) for defining automation tasks, plus an interactive web UI for exploring and recording actions. Primary target is [[ExportMaster]] automation.
