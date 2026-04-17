# ONI-Mods

A [[CSharp]] monorepo of [[GameMods]] for [[OxygenNotIncluded]] — enhanced storage tooltips, infinite-storage cheats, automation helpers, and a handful of convenience tweaks.

**Repo:** `~/Git/ONI-Mods`

Each mod is a self-contained subfolder building against the game's Unity / .NET Framework 4.7.2 assemblies via MSBuild. The only mod currently shipped to the Steam Workshop is Storage Tooltip; the rest (magic-storage, critter-dispatch, dupe-therapist, auto-teleport, pipe-overlay, oni-repl and more) are at varying stages of WIP. Sibling project [[StinkySpy]] provides the data layer that informs a lot of the modding decisions here.
