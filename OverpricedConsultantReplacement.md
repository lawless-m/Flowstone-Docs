# OverpricedConsultantReplacement

"OCR: Overpriced Consultant Replacement" — a production-ready [[python]] invoice OCR service using PaddleOCR and Unstructured.io to extract structured data from supplier PDFs, with GPU/CPU switching so it can either answer demo queries in seconds or chew through batches on the CPU while the GPU is busy elsewhere.

**Repo:** `~/Git/OverpricedConsultantReplacement`
**Themes:** [[python]]

FastAPI backend behind Nginx, plus a small drag-and-drop web frontend. Extracts invoice number, dates, totals, supplier and customer, line items with VAT analysis, and confidence scores. Supplier-specific templates for known vendors with fallback to generic parsing, table parsing for line items, multi-currency (GBP / USD / EUR), works with both native and scanned PDFs. GPU mode runs in 2–5 seconds per invoice, CPU mode in 10–30 — switchable per request via checkbox or API flag, no service restart. Ships with a systemd + Nginx + Apache2 deployment recipe and runs happily behind an Apache reverse proxy at `/OCR/`. Name is a joke about the cost of the consultants it replaces.

## Related

- [[python]]
