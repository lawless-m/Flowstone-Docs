# InvalidQuoteIdFinder

A [[RocsMiddleware]] diagnostic tool that detects broken quote references in [[ElasticSearch]] shipment records.

**Repo:** `~/Git/RocsMiddleware/InvalidQuoteIdFinder`

Takes a customer code, queries all their shipments in [[ElasticSearch]], checks each quote ID reference exists in the `quotes` index, and outputs a JSON report of invalid references. Ad-hoc tool, not scheduled.
