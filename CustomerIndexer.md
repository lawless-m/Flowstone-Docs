# CustomerIndexer

A [[RocsMiddleware]] service that incrementally syncs customer data from [[ExportMaster]] and PostgreSQL into [[elasticsearch]].

**Repo:** `~/Git/RocsMiddleware/CustomerIndexer`

Combines ExportMaster customer profiles with CRM data from PostgreSQL, uses hash-based change detection to index only changed customers, and automatically removes obsolete records from Elasticsearch.
