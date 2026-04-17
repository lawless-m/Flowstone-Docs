# MasterBlaster

A [[CSharp]] desktop automation engine that drives legacy Windows apps over RDP using Claude vision.

**Repo:** `~/Git/MasterBlaster`

MasterBlaster captures screenshots from an RDP session, sends them to [[Claude-API]] for visual analysis, and executes mouse/keyboard actions based on what Claude identifies on screen. Has a custom declarative language (MBL) for defining automation tasks, plus an interactive web UI for exploring and recording actions. Primary target is [[ExportMaster]] automation.
