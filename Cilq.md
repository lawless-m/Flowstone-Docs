# Cilq

A [[CSharp]] / [[Dotnet]] WebSocket bridge — "Claude Browser Bridge" — that lets Claude Code drive a live browser: capture console logs, track JavaScript errors and stack traces, and execute arbitrary scripts in any open tab from the command line. The server side of the BrowserBridge pattern that appears as a skill in [[Claude-Skills]].

**Repo:** `~/Git/Cilq`

Three components. An ASP.NET Core bridge server listening on `localhost:3141` with an HTTP API for Claude Code and a WebSocket endpoint for browser connections. A Chrome/Edge browser extension that installs a content script to capture `console.*` calls, uncaught exceptions and unhandled promise rejections, streaming them up to the server in real time. And a planned Claude Code integration layer (MCP server or native tool). Use case: Claude is driving a web frontend you're building, runs `curl /api/browser/execute` with a JavaScript snippet, and gets real-time DOM state back without leaving the terminal.
