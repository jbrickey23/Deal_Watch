# Deal_Watch — Sources

This file defines the source checklist and reporting expectations across active Deal_Watch domains. Source accessibility can change; preserve observed status rather than assuming permanent access.

## Primary discovery sources

- eBay — large used market, exact model searches, photos, sold-price context; historically the most reliable source.
- Craigslist — local bargains, older equipment/gear, sellers who may not know exact model/value.
- OfferUp — local used gear and garage-sale-type finds; access may be variable.
- Facebook Marketplace — potentially excellent for genuine local bargains; often limited without login or direct marketplace access.
- Mercari — consumer-to-consumer used gear and occasional mispricing.
- EstateSales.net — estate inventories, lots, and poorly identified older equipment/gear.
- BidRush — local/estate-style auctions with item pages that can expose title, description, bid state, location, dates, pickup/shipping status, photos, and auction metadata.

## Domain-specific discovery sources

### Hat:Machine
- **ForSewing.us** — industrial sewing-machine dealer/source to search for purpose-built hat/sweatband machines and convertible/sleeper industrial machines, especially cylinder-bed, post-bed, free-arm/off-the-arm, walking-foot, and older/discontinued specialty machines. Also use for model identification, specifications, parts/attachment availability, and price benchmarking when appropriate. Do not treat a dealer description that a machine sews leather as proof of sweatband suitability; apply the Hat:Machine geometry/modification-feasibility test.

## Secondary discovery sources

- GoodwillFinds — donated gear and obscure models.
- ShopGoodwill — auctions and treasure-hunt potential.
- American Legacy Fishing — used/trade-in premium fishing rods, especially Shimano and G. Loomis.

## Retail baseline / verification sources

- Tackle Warehouse — current fishing pricing/spec comparison and clearance context.
- FishUSA — Fenwick/Shimano pricing, sales, and closeouts.
- Manufacturer sites — exact model/SKU, specification, MSRP, generation confirmation, manuals and application documentation.
- Specialty industrial sewing dealers and parts suppliers — machine specifications, application information, parts/feet/guides availability, and price benchmarks for Hat:Machine.

## Broader-web discovery

Search the broader web where practical for:
- independent specialty shops/dealers
- pawn shops
- liquidation/closeout inventory
- forgotten old stock
- poorly indexed specialty retailers

These can produce the closest thing to true `garage finds` online.

## Source-role distinction

### Discovery
Used to find actionable listings.

### Verification
Used to establish exact model/SKU, generation/year, configuration/specifications, visible condition, seller claim versus evidence, original/current equivalent price, realistic used value, shipping/delivered price, transaction risk, and—where applicable—Hat:Machine geometry and modification feasibility.

A source used only for verification must not be reported as a searched marketplace source.

## Required run coverage reporting

Every substantive run should include a compact coverage footer or equivalent.

Allowed source-run states:
- `SEARCHED` — source was actually queried/inspected during this run.
- `INACCESSIBLE` — attempted but unavailable or blocked sufficiently that meaningful search could not be completed.
- `NOT SEARCHED` — source was intentionally or practically omitted from this run.

Never report `no deals found` for a source that was not actually searched.

## Current evidence about accessibility

As of initialization on 2026-09-13:
- eBay: successfully searched in prior manual runs.
- manufacturer/retailer sites: successfully used for verification.
- Facebook Marketplace: known access limitation in prior discussion; treat as unverified/inaccessible until a run proves otherwise.
- Craigslist, OfferUp, Mercari, EstateSales, Goodwill sources, pawn shops, and independent specialty shops: included in the desired search universe but not yet consistently validated in the durable workflow.

As of 2026-09-15:
- BidRush direct item pages were validated as readable and capable of exposing useful listing data. Treat BidRush as a promising source; broader search coverage still needs validation in future runs.

As of 2026-09-16:
- ForSewing.us added as an explicit Hat:Machine discovery and verification source. Accessibility/search quality should be validated on subsequent Hat:Machine runs.

`FDW-TODO-001` owns systematic validation of this matrix; the legacy ID is intentionally preserved.
