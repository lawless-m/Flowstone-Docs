# Nawin

A [[CSharp]] / [[dotnet]] 9 implementation of the [[9P]]2000 protocol for connecting to [[Plan9]] and 9front file servers — a full wire-protocol client and server library with both legacy (p9sk1) and modern (dp9ik) authentication.

**Repo:** `~/Git/Nawin`

Ships as a set of .NET 9 libraries (Nawin.Protocol, Nawin.Transport, Nawin.Client, Nawin.Server), a CLI with ls / cat / stat / write / mkdir / rm / interactive shell, and a 157-test suite. Zero external dependencies beyond System.CommandLine. Async/await throughout. A natural complement to [[Crabbit]], which implements the same `/net` server model from Rust for a very different purpose — Crabbit serves a WireGuard tunnel as `/net`, Nawin consumes and serves 9P trees generally.
