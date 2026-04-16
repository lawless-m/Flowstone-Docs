# Crabbit

A [[Rust]] userspace WireGuard peer that exposes its tunnel as a [[9P]] `/net` filesystem, letting any [[Plan9]] system join a WireGuard mesh by simply importing `/net` from Crabbit.

**Repo:** `~/Git/Crabbit`

Plan 9 networks by importing `/net` from somewhere and using it. WireGuard doesn't speak 9P and Plan 9 doesn't speak WireGuard — Crabbit bridges the gap. It handles the WireGuard protocol in userspace, joins an existing mesh as a peer, and presents the tunnel as a proper Plan 9 `/net` with native p9sk1 authentication. Self-contained single binary, no kernel involvement on the host. Written in Rust with maximum ceremony to serve Plan 9's maximum simplicity. Currently in development — project skeleton and 9P version negotiation are in place; the WireGuard integration, `/net` engine, auth and DNS pieces are still being built.
