# boofuzz-iscsi

A [[python]] [[fuzzing]] harness that acts as a malicious [[iSCSI]] initiator, sending malformed PDUs to an iSCSI target to flush out buffer overflows, integer-overflow length-handling bugs, state-machine violations and memory corruption in key=value parsing.

**Repo:** `~/Git/boofuzz-iscsi`
**Themes:** [[python]], [[iSCSI]], [[fuzzing]]

Built on the boofuzz framework. Supports full-session fuzzing or a faster login-only mode for initial testing, exposes boofuzz's web interface on localhost:26000 to watch progress, and carries its own PDU definitions for login requests, SCSI commands, text/nop/logout opcodes. Companion to [[VoE]] (the Venti-over-Ethernet target this fuzzer can hammer) and [[iscsi-crate]] (the pure-Rust target library). Together the three form the iSCSI cluster in this corpus.
