# NASty

A hardware-focused project whose folder structure — `HARDWARE.md`, `PLANNING.md`, `CONTENTS.md`, `mtd-backup/`, `pxe/`, `proc.cpuinfo`, `proc.mtd`, `test-armel/` — strongly suggests an embedded-Linux / NAS firmware hack, probably flashing or net-booting a cheap ARM NAS device. "NASty" is the obvious pun.

**Repo:** `~/Git/NASty`

Design and reconnaissance files are in place: `HARDWARE.md` (4 KB) and `PLANNING.md` (3 KB) describing the intent, `proc.cpuinfo` and `proc.mtd` dumped from the target device, a backup of the original MTD (flash) partitions in `mtd-backup/`, a PXE boot tree in `pxe/`, and `test-armel/` suggesting ARM EABI experimentation. No README at the repo root. **Status:** unclear whether actual flashing or TFTP boot has been attempted yet — needs a read of `HARDWARE.md` next pass to identify the specific hardware and rewrite this note from fact.
