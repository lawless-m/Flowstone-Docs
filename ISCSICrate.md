# iscsi-crate

A pure [[Rust]] [[ISCSI]] target library with a trait-based storage backend — users implement `ScsiBlockDevice` for their own in-memory, file, or network-attached storage, and the crate handles all iSCSI and SCSI protocol details.

**Repo:** `~/Git/iscsi-crate`

Supports login/logout/discovery/normal sessions, the full block-command set (READ/WRITE 6/10/16, INQUIRY, READ CAPACITY, TEST UNIT READY, MODE SENSE, SYNCHRONIZE CACHE, REQUEST SENSE, REPORT LUNS, VERIFY), CHAP authentication (one-way and mutual), SendTargets discovery, and multi-PDU Data-Out writes. Verified in the real world against Linux open-iscsi and `iscsiadm`. Builder-pattern API. The library side of the iSCSI triangle formed with [[VoE]] (target server) and [[BoofuzzISCSI]] (fuzzer) — together they give you your own target, a real client, and a hostile one, which is a nice setup for testing anyone's iSCSI implementation.
