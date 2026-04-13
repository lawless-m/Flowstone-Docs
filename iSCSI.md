# iSCSI

The iSCSI protocol cluster. Matt has the full triangle: a target server, a target library for building custom targets, and a protocol fuzzer that can attack any target. Together they make a reasonable test bench for anyone's iSCSI stack.

## Members

- [[VoE]] — Venti-over-Ethernet network block storage, iSCSI is one of its supported protocols
- [[iscsi-crate]] — pure-Rust iSCSI target library with a trait-based storage backend
- [[boofuzz-iscsi]] — malicious-initiator iSCSI fuzzer for finding bugs in any target

## Related themes

- [[Plan9]] — VoE is a Venti homage
- [[fuzzing]]
- [[rust]]
