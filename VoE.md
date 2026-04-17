# VoE

A suite of [[Rust]] network block storage servers — "Venti over Ethernet", a [[Plan9]] homage to Venti, Bell Labs' content-addressed archival store — with pluggable protocols ([[AoE]], NBD, [[ISCSI]]) and a CAS backend that does block-level deduplication and immutable snapshots.

**Repo:** `~/Git/VoE`

The CAS backend is the Venti model with a modern hash: immutable content-addressed blocks with a Merkle-tree index, BLAKE3 instead of Venti's SHA-1, LZ4 compression on top. Unique blocks land at roughly 120 MB/s, duplicates at 500 MB/s. Pluggable blob stores (file system, S3, Azure, Backblaze B2) sit behind a trait. VoE then exposes the store over the wire as ordinary disk images so standard OS initiators can mount them without any special client software; multi-target support means one server can host multiple shelves and slots. The iSCSI path bridges through a TGT+NBD combo for Windows clients. Natural neighbour to [[Boofuzz-ISCSI]] and [[ISCSI-Crate]] on the iSCSI side, and to [[Crabbit]] and [[Nawin]] on the Plan 9 side.
