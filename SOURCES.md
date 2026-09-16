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

### Hat:Machine — industrial sewing dealers / used machinery
- **ForSewing.us** — search for purpose-built hat/sweatband machines and convertible/sleeper industrial machines, especially cylinder-bed, post-bed, free-arm/off-the-arm, walking-foot, and older/discontinued specialty machines. Also use for identification, specs, parts/attachments and price benchmarks.
- **SewingMachinery.com used equipment** — substantial used-industrial inventory organized by machine architecture, including walking-foot/heavy-duty, post-bed, cylinder-arm, feed-up-arm/feed-off-arm and special-purpose/old-special machines. Search both exact models and architectural categories.
- **C.H. Holderby used machines** — Seattle-area industrial sewing dealer with changing used inventory. Especially important because machines may be inspectable/pickup-accessible from the 98053 search base and the dealer can evaluate a material/application sample.
- **Sewman / American Sewing Machine** — new and used factory/industrial machines, including upholstery/walking-foot equipment; useful for sleeper discovery, comparable models, parts and price baselines.
- **Atlas Levy** — industrial sewing dealer with new and used inventory, repair/service and parts; search for used cylinder/post/specialty machines and comparable configurations.
- **Stitch Machine Ledger marketplace / used-machine research** — used-market and price-context source spanning industrial, leather/bag, upholstery/canvas and specialty machines. Use as discovery/market intelligence where actual listings are available and as verification otherwise.

### Hat:Machine — adjacent trade / upholstery / leather discovery
Do not restrict searches to sellers using `hat` or `sweatband`. Search used-equipment inventories and classifieds serving:
- automotive and furniture upholstery shops;
- marine canvas/awning shops;
- leather-goods and bag makers;
- shoe/boot repair and cobbler shops;
- textile/apparel factories and shop liquidations;
- millinery/hat-shop closures;
- industrial sewing repair dealers and mechanics selling trade-ins;
- business-liquidation and surplus-equipment auctions.

These adjacent trades are high-value sleeper territory because cylinder-arm, post-bed, walking-foot, feed-off-arm and specialty machines may be listed by their former trade rather than by machine architecture or hat suitability.

### Hat:Machine source-search behavior
Search by both application and architecture. Include terms such as `used upholstery sewing machine`, `upholstery shop equipment`, `industrial walking foot`, `cylinder arm`, `cylinder bed`, `post bed`, `off the arm`, `feed off arm`, `free arm industrial`, `leather sewing machine`, `cobbler machine`, `shoe repair sewing machine`, `canvas sewing machine`, `awning sewing machine`, `bag sewing machine`, `industrial sewing shop liquidation`, and poorly identified `industrial sewing machine` listings.

Do not treat `sews leather`, `upholstery`, or `walking foot` as proof of sweatband suitability. Every Hat:Machine candidate still receives the geometry/modification-feasibility test: can a formed felt hat rotate around the sewing point, can the seam reach the crown/brim junction, and can feet/guides/needle/table/drive be modified economically enough to make the operation practical?

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

Search the broader web where practical for independent specialty shops/dealers, sewing-machine mechanics, upholstery/leather/canvas shop liquidations, pawn shops, business auctions, liquidation/closeout inventory, forgotten old stock, and poorly indexed specialty retailers. These can produce the closest thing to true `garage finds` online.

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
- ForSewing.us added as an explicit Hat:Machine discovery and verification source.
- SewingMachinery.com exposes a broad used-industrial inventory organized by architecture, including cylinder arm, post bed, walking foot/heavy duty, feed-up/off-arm and special-purpose machines.
- C.H. Holderby exposes changing used industrial inventory from Seattle, WA and is especially relevant for local inspection/application testing.
- Sewman/American Sewing Machine and Atlas Levy expose industrial machine inventory useful for discovery and benchmarks.
- Stitch Machine Ledger exposes industrial/leather/upholstery used-market research and marketplace functions useful for broader discovery and price context.
- Upholstery, marine canvas, leather/bag, shoe-repair and shop-liquidation sources are explicitly in-scope as sleeper discovery channels.

`FDW-TODO-001` owns systematic validation of this matrix; the legacy ID is intentionally preserved.
