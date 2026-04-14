# Dingo

A web-based Australian biosecurity compliance declaration generator that replaces an Excel/Word workflow with interactive PDF output.

**Repo:** `~/Git/Dingo`
**URL:** `https://dw.ramsden-international.com/tiny02/dingo.html`
**Themes:** [[javascript]], [[DBISAM]], [[HTMLDataTable]]

Dingo automates the creation of Food Label Declarations, Supplier Declarations, and Product Specification Declarations for imported food shipments. It pulls shipment data from a [[DBISAM]] backend via [[HTMLDataTable]], auto-detects ingredient categories (dairy, eggs, gelatine, pork, beef) from product descriptions, and generates compliant PDF documents using pdfMake. Deployed as a static HTML app on [[dw.ramsden-international.com]] with a vanilla JS frontend — no frameworks.
