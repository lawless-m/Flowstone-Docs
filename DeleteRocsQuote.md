# DeleteRocsQuote

A [[RocsMiddleware]] manual tool for deleting unordered quotes and shipments from [[ElasticSearch]].

**Repo:** `~/Git/RocsMiddleware/DeleteRocsQuote`

Searches quotes and shipments in [[ElasticSearch]], checks for order dependencies before deletion, and supports both interactive CLI confirmation and automated flags. Validates shipment (`A-NN-NNNNNN`) and quote (`EQNNNNNN`) patterns.
