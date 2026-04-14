# DBISAM

The file-based database engine behind [[ExportMaster]]. Accessed via ODBC or the ExportMaster COM DLL. Files use `.dat`, `.idx`, and `.blb` extensions on a network share.

## Members

- [[ExportMaster]] — the application that owns the DBISAM database
- [[CGI-Sharp]] — queries DBISAM tables via ODBC
- [[HTMLDataTable]] — the CGI executable serving DBISAM data as JSON
- [[Dingo]] — consumes DBISAM data via HTMLDataTable
- [[EMUpdater]] — writes back to DBISAM via COM DLL
- [[Gravedigger]] — creates non-intrusive VSS backups of DBISAM files
- [[PowerQueries]] — Power Query modules reading DBISAM via ODBC
- [[RocsMiddleware]] — several children read from DBISAM

## Related themes

- [[ODBC]] — primary read access method
- [[ExportMaster]] — the application layer above DBISAM
- [[FakeODBC]] — a mock ODBC driver that mimics a DBISAM data source
