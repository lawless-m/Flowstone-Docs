# FixErlang

A write-up, patch and implementation plan for an AddressSanitizer memory leak in Erlang/OTP's `erts/etc/unix/dyn_erl.c`, discovered while building an ASAN-instrumented Erlang VM for [[Fuzzing]] EMQX (an Erlang MQTT broker).

**Repo:** `~/Git/FixErlang`

Not a project in the usual sense — a single-issue repo documenting a bug hunt. Root cause: `find_prog()` in `dyn_erl.c:209` returns a `strdup()`'d string that the caller must free, and the `--realpath` code path (lines 365–373) exits early without the `efree(abspath)` call. The fix is a single line added before the early return. The repo holds the patched source, an `0001-Fix-memory-leak-in-dyn_erl.c-find_prog.patch` file ready for upstream submission, and an implementation checklist that's complete through "build Erlang with fix + ASAN enabled and verify no leak reports"; the final steps ("fork erlang/otp, submit PR") are not yet checked off. The motivation comes from [[Mtqq-Fuzzer]]: ASAN is needed to detect memory errors in EMQX's C NIFs during MQTT fuzzing, and the ASAN build was failing on this upstream leak.
