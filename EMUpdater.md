# EMUpdater

A [[RocsMiddleware]] service that pushes customer and discount data from PostgreSQL back into [[ExportMaster]] via its COM DLL.

**Repo:** `~/Git/RocsMiddleware/EMUpdater`
**Themes:** [[csharp]], [[dotnet]], [[ExportMaster]], [[DBISAM]]

Generates XML in PostgreSQL stored procedures and submits it to the ExportMaster COM interface (`ECNICI.E3CustomerInterface`). Builds as 32-bit (x86) due to COM DLL compatibility. Routes to different EM servers based on machine name.

## Related

- [[RocsMiddleware]]
- [[ExportMaster]]
- [[DBISAM]]
