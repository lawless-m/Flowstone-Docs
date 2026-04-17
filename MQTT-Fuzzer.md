# MQTT-Fuzzer

A [[Python]] [[Fuzzing]] harness — "MQTT 3.1.1 Protocol Fuzzer for boofuzz" — for testing MQTT broker implementations against the OASIS spec. The repo name is a deliberate transposition of MQTT.

**Repo:** `~/Git/mtqq-fuzzer`

Built on boofuzz, like its iSCSI sibling [[Boofuzz-ISCSI]]. Covers the full MQTT 3.1.1 packet set: CONNECT, PUBLISH at QoS 0/1/2, SUBSCRIBE and UNSUBSCRIBE, PING, DISCONNECT, and the full QoS handshake (PUBACK / PUBREC / PUBREL / PUBCOMP). Edge cases include malformed UTF-8, invalid remaining-length encoding, oversized packets, duplicate CONNECT, reserved-bit abuse and wildcard (`+`, `#`) abuse in invalid positions. Target was Eclipse Mosquitto running under Docker, with an ASAN-instrumented build path for serious vulnerability hunting. That ASAN build path is what led to the [[FixErlang]] side quest: the Erlang-based EMQX broker's ASAN build kept crashing on an unrelated memory leak upstream in Erlang/OTP itself. Ships with a full Dockerfile for the ASAN mosquitto build and coverage tables for every packet type the fuzzer exercises. Motto borrowed from the README: *"the S in IoT stands for Security."*
