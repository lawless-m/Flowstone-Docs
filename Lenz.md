# Lenz

A [[csharp]] Windows Explorer preview handler spec for the Prysm ProjFS virtual filesystem, rendering metadata as HTML via WebView2.

**Repo:** `~/Git/Lenz`
**Themes:** [[csharp]], [[dotnet]]

Lenz adds a preview pane to Windows Explorer for files in the `C:\Prysm` projected filesystem. A COM preview handler DLL communicates with the Prysm ProjFS provider over named pipes, which queries PostgreSQL for metadata and returns HTML rendered in WebView2. Includes a mock pipe server for isolated testing.
