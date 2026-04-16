# Plaster1-WorkInvoice

A [[CSharp]] tool that queries [[ExportMaster]] for repro shipment data and populates workload-invoice Excel templates on [[SharePoint]].

**Repo:** `~/Git/Plaster1-WorkInvoice`

Plaster1-WorkInvoice pulls non-invoiced orders and quotes from [[ExportMaster]] via [[ODBC]], then uses the Microsoft Graph API to upload and populate Excel workbooks on [[SharePoint]] (ramsdenint.sharepoint.com). Handles effort/capacity calculation across 18 repro product types, range code mapping, and a 27-flag system for product attributes. Authenticates via Azure AD.
