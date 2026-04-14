# Cuthbert

A cross-platform [[rust]] network topology visualiser that renders the local routing table as an interactive 3D graph, traces routes to arbitrary destinations, and auto-discovers other nodes on the same mesh.

**Repo:** `~/Git/Cuthbert`
**Themes:** [[rust]], [[cli-tools]]

Built to answer the kind of question that comes up when you run multiple overlapping VPN tunnels: which tunnel does traffic to destination X actually use, can machine A reach machine K, is the VPN path faster than the public internet, why can't two machines communicate. The tool spins up a local web server, displays routes radiating from your machine in a three.js 3D graph colour-coded by latency, and can perform on-demand bandwidth testing between discovered nodes. Runs on Linux, Windows and macOS; currently in development.
