# Prysm

A [[CSharp]] ProjFS virtual filesystem that presents product images through multiple computed views without duplicating files.

**Repo:** `~/Git/Prysm`

Prysm mounts a Windows Projected File System at `C:\Prysm` backed by PostgreSQL stored procedures. The same physical image files appear under multiple directory views — by barcode, product code, order number, or shipment reference — with on-demand resizing and format conversion (jpg/png/webp at multiple sizes). Runs as a Windows Service on Server 2022, accessible over standard SMB. Includes a write-enabled ingest path for validated uploads and a PostgreSQL LISTEN/NOTIFY system for real-time change propagation. [[Lenz]] adds an Explorer preview handler on top.
