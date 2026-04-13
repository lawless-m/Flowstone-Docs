# Fuzzing

Protocol fuzzers and related bug-hunt work in this corpus. Matt's fuzzing targets embedded or network protocols via the boofuzz framework, with occasional side quests into the fuzzed targets' toolchains when their AddressSanitizer builds fall over.

## Members

- [[boofuzz-iscsi]] — iSCSI target fuzzer, hammers [[VoE]] and [[iscsi-crate]]
- [[mtqq-fuzzer]] — MQTT 3.1.1 broker fuzzer targeting Mosquitto (and EMQX)
- [[FixErlang]] — Erlang/OTP memory-leak fix, surfaced while building an ASAN Erlang VM to fuzz EMQX

## Related themes

- [[iSCSI]]
- [[python]]
