# Deal_Watch — Fishing Sources

This file defines the source checklist and reporting expectations for the current fishing watch domain. Source accessibility can change; preserve observed status rather than assuming permanent access.

## Primary discovery sources

- eBay — large used market, exact model searches, photos, sold-price context; historically the most reliable source.
- Craigslist — local bargains, older rods, sellers who may not know exact model/value.
- OfferUp — local used gear and garage-sale-type finds; access may be variable.
- Facebook Marketplace — potentially excellent for genuine local bargains; often limited without login or direct marketplace access.
- Mercari — consumer-to-consumer used gear and occasional mispricing.
- EstateSales.net — estate inventories, lots, and poorly identified older fishing gear.
- BidRush — local/estate-style auctions with item pages that can expose title, description, bid state, location, dates, pickup/shipping status, photos, and auction metadata; promising for both fishing gear and future thrift/upcycle domains such as felt hats.

## Secondary discovery sources

- GoodwillFinds — donated rods/reels and obscure models.
- ShopGoodwill — auctions and fishing lots with treasure-hunt potential.
- American Legacy Fishing — used/trade-in premium rods, especially Shimano and G. Loomis.

## Retail baseline / verification sources

- Tackle Warehouse — current pricing/spec comparison and clearance context.
- FishUSA — Fenwick/Shimano pricing, sales, and closeouts.
- Manufacturer sites — exact model/SKU, specification, MSRP, and generation confirmation.

## Broader-web discovery

Search the broader web where practical for:
- independent tackle shops
- pawn shops
- liquidation/closeout inventory
- forgotten old stock
- poorly indexed specialty retailers

These can produce the closest thing to true `garage finds` online.

## Source-role distinction

### Discovery
Used to find actionable listings.

### Verification
Used to establish:
- exact model number/SKU
- generation/year
- configuration/specifications
- visible condition
- seller claim versus photographic evidence
- original/current equivalent price
- realistic used value
- shipping/delivered price
- seller/transaction risk

A source used only for verification must not be reported as a searched marketplace source.

## Required run coverage reporting

Every substantive run should include a compact coverage footer or equivalent, for example:

`Sources checked: eBay SEARCHED | Craigslist SEARCHED | OfferUp SEARCHED | Mercari SEARCHED | EstateSales SEARCHED | BidRush SEARCHED | Facebook INACCESSIBLE | ShopGoodwill SEARCHED`

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
- Craigslist, OfferUp, Mercari, EstateSales, Goodwill sources, pawn shops, and independent tackle shops: included in the desired search universe but not yet consistently validated in the durable workflow.

As of 2026-09-15:
- BidRush: direct item page `https://bidrush.com/items/vintage-men-s-hats-KYK5H9` returned `200 OK` from workspace fetch. The page embedded useful listing data including title, description, location, status, end time, highest bid, bid count, pickup/shipping flags, and image URLs. Treat BidRush as a promising validated source for direct listing reads; broader search coverage still needs validation in future runs.

`FDW-TODO-001` owns systematic validation of this matrix; the legacy ID is intentionally preserved.
