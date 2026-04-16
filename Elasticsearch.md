# ElasticSearch

ElasticSearch 5.2 search clusters — production and staging — used for product, customer, pricing, and quote search across the [[ROCS]] platform.

Hosted on [[AWS]] and stuck on an old version. Genius.

Two clusters:
- **Production:** `rocs-production-es.ramsden-international.com`
- **Staging:** `rocs-stage-es.ramsden-international.com`

Key indexes: `price_discount`, `customers`, `quotes`, `shipments`, `orders`.
