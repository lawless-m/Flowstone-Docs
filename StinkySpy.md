# StinkySpy

A [[rust]] production-chain calculator for [[Oxygen-Not-Included]], built on building data extracted straight from the decompiled game source rather than wiki approximations.

**Repo:** `~/Git/StinkySpy`
**Themes:** [[rust]], [[Oxygen-Not-Included]], [[SQLite]], [[claude-tooling]]

The calculator stores buildings, resources, power, heat and throughput rates in [[SQLite]] and answers production-chain questions ("how many electrolysers for a hydrogen generator?", "which generator runs coolest per watt?"). The intended front end is Claude itself: the database is the backend, Claude is the query interface. StinkySpy also ships a small set of Claude Code skills covering ONI calculator usage, skill-building, database access and logging. It is the data-layer sibling to [[ONI-Mods]].
