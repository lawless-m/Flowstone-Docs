# DrX3

A [[csharp]] database detective for Sage X3 ERP — extracts schema, discovers relationships, and generates ERD diagrams.

**Repo:** `~/Git/DrX3`

DrX3 (X3Detective) analyses Sage X3 SQL Server databases by extracting full DDL, then discovering foreign key relationships through index pattern analysis, naming conventions, and data sampling validation. Stores discovered metadata in [[MongoDB]] and outputs diagrams in Mermaid, Graphviz, and D2 formats. Includes a cross-table value finder with multiple search modes for tracing data across the ERP schema.
