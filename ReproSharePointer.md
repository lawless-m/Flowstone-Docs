# ReproSharePointer

A [[csharp]] tool that uploads seasonal product images to [[SharePoint]] and updates an Excel tracker via the Graph API.

**Repo:** `~/Git/ReproSharePointer`
**Themes:** [[csharp]], [[dotnet]], [[SharePoint]]

ReproSharePointer reads a master artwork samples tracker spreadsheet from [[SharePoint]], finds matching product images on a network share, uploads them, and updates the tracker with links. Handles duplicate detection, dry-run simulation, automatic folder creation, and sends email reports with zipped logs. Authenticates via Azure Entra ID.

## Related

- [[Plaster1-WorkInvoice]] — sibling repro workflow tool
- [[csharp]]
- [[dotnet]]
- [[SharePoint]]
