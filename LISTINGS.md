# Deal_Watch — Fishing Listing History

This is the durable ledger for notable listings and market observations in the current fishing watch domain. It is not intended to contain every search result; preserve items that matter for future comparison, status tracking, or deal-rule calibration.

Newest observations first.


## 2026-09-13 — Second specification-driven search run

**Run result:** No new actionable listing met the notification threshold. Named targets and specification-driven candidates were searched across the public/indexed portions of the source set.

### Shimano Stradic FM ST2500HGFM — TackleAnglers indexed offer
**Status:** REJECTED / HIGH TRANSACTION RISK  
**Indexed price:** $63.75, purportedly reduced from $254.99  
**Exact model confidence:** High from the indexed product title; live inventory and fulfillment unverified  
**Deal Score:** Not scored as an actionable acquisition

Assessment: the indexed price is roughly 75% below the normal $254.99 retail benchmark and would be exceptional if legitimate, but the storefront returned HTTP 403 during validation and no independent evidence established current stock, seller reliability, authorized-dealer status, shipping, or buyer protection. Do not treat this as a deal alert without direct verification of the merchant and checkout protections.

### Current-market reel benchmarks
- ST2500HGFM: multiple established U.S. retailers and an eBay dealer were observed at $254.99, reinforcing that the $63.75 indexed result is an extreme outlier rather than an ordinary promotion.
- ST1000HGFM: established retail observations remained around $234.99. An overseas listing at €159.79 was observed, but international delivery cost, warranty, and import risk were not established; it did not clear the actionable threshold.

### Other observations
- Facebook Marketplace public indexing exposed a G. Loomis IMX-Pro bladed-jig rod at $300, but the page was login/temporary-block limited and the rod did not match the current Medium-Light/Medium specification profile closely enough to pursue.
- EstateSales.net exposed a future fishing-tackle sale containing Loomis and Shimano items, but exact models, condition, individual prices, and actionable purchase details were unavailable.
- American Legacy Fishing / The Rod Locker exposed active used inventory categories, including G. Loomis and Poison Adrena, but the public result did not establish a qualifying configuration at bargain pricing.
- Retail checks reconfirmed Fenwick Eagle EGLW70ML-FS-2 near $99.95–$99.99 and Fenwick HMG HMGW72ML-FS-2 near $179.95. These remain benchmarks rather than alerts.

### Source coverage — this run

Coverage reflects public web/domain-indexed access, not exhaustive authenticated marketplace inventory.

- eBay — SEARCHED; indexed listings and current price results inspected.
- Craigslist — SEARCHED; public indexed search attempted, no worthwhile current result surfaced.
- OfferUp — SEARCHED; public indexed search attempted, no worthwhile current result surfaced.
- Mercari — SEARCHED; public indexed search attempted, no worthwhile current result surfaced.
- EstateSales.net — SEARCHED; one broad sale result surfaced, but insufficient item-level detail.
- Facebook Marketplace — INACCESSIBLE; limited indexed result surfaced, but meaningful inventory inspection was blocked.
- GoodwillFinds — SEARCHED; public indexed search attempted, no worthwhile result surfaced.
- ShopGoodwill — SEARCHED; public indexed search attempted, no worthwhile result surfaced.
- American Legacy Fishing / The Rod Locker — SEARCHED; used inventory page inspected, no verified bargain surfaced.
- Manufacturer/retailer sources — SEARCHED for verification and current benchmarks, not marketplace discovery.
- Independent tackle/pawn/liquidation broader web — SEARCHED on a limited indexed basis; one extreme-price storefront result was rejected for verification and transaction-risk reasons.


## 2026-09-13 — First specification-driven search run

**Run result:** No new actionable listing met the notification threshold. The reorganized rod search did successfully surface models/configurations from their specifications rather than relying only on the pre-existing named-model list.

### Fenwick Eagle Walleye specification family — FishUSA retail verification
**Status:** BENCHMARK / specification-discovery validation  
**Price:** $99.99 new at observation  

Matching 2-piece configurations discovered/verified within the broad preferred envelope included:
- `EGLW63ML-XFS-2` — 6'3", Medium Light, Extra Fast, 2-piece
- `EGLW66M-FS-2` — 6'6", Medium, Fast, 2-piece
- `EGLW69ML-XFS-2` — 6'9", Medium Light, Extra Fast, 2-piece
- `EGLW70ML-FS-2` — 7'0", Medium Light, Fast, 2-piece
- `EGLW70M-XFS-2` — 7'0", Medium, Extra Fast, 2-piece

Assessment: these are not bargain alerts at roughly $100 new, but they validate the new specification-driven discovery approach and provide useful new-price anchors for used listings.

### Fenwick Eagle EGLB66M-XFS-2 — Tackle Warehouse retail verification
**Status:** BENCHMARK / newly surfaced configuration  
**Price:** $99.95 new at observation  
**Configuration:** 6'6", Medium, Extra Fast, 2-piece  

Assessment: exact match to the broad preferred construction/length/power/action envelope. Useful baseline; ordinary used examples need a meaningful discount from ~$100 new to become interesting.

### Shimano 2026 Zodias 268ML-2 — eBay retail/import listing
**Status:** OBSERVED / specific-target benchmark  
**Price:** $224.34 new at observation  
**Configuration verified from listing:** 6'8", Medium Light, 2-piece; action not independently established during this run  

Assessment: fits most broad physical criteria and the Zodias priority family, but observed new price is not a bargain signal. Preserve as a current-market reference only.

### Shimano Zodias 164L-BFS/2 — eBay
**Status:** REJECTED / out-of-envelope  
**Price:** $173.84 used, free shipping at observation  

Assessment: active used two-piece Zodias listing, but Light power is outside the current Medium-Light/Medium preferred search envelope and the price does not create an exceptional-value reason to override that preference.

### Source coverage — this run

Coverage reflects what was actually queryable through public web indexing/search in this ChatGPT run; it does not imply authenticated/native marketplace access.

- eBay — `SEARCHED`; multiple current/indexed listings and category results inspected.
- Craigslist — `SEARCHED`; public indexed search attempted, no worthwhile result surfaced.
- OfferUp — `SEARCHED`; public indexed search attempted, no worthwhile result surfaced.
- Mercari — `SEARCHED`; public indexed search attempted, no worthwhile result surfaced.
- EstateSales.net — `SEARCHED`; public indexed search attempted, no worthwhile result surfaced.
- Facebook Marketplace — `INACCESSIBLE`; public search did not provide meaningful marketplace inventory access.
- GoodwillFinds — `SEARCHED`; public indexed search attempted, no worthwhile result surfaced.
- ShopGoodwill — `SEARCHED`; public indexed search attempted, no worthwhile result surfaced.
- American Legacy Fishing — `SEARCHED`; public indexed search attempted, no worthwhile result surfaced.
- Tackle Warehouse — `SEARCHED` for retail/specification verification, not counted as marketplace discovery.
- FishUSA — `SEARCHED` for retail/specification verification, not counted as marketplace discovery.
- Independent tackle/pawn/liquidation broader web — `NOT SEARCHED` systematically in this run.

Operational note: this run demonstrates that broad web/domain-indexed searching can validate several sources, but `SEARCHED` via public indexing is not equivalent to exhaustive native-site inventory coverage. Future runs should continue testing source reliability under `FDW-TODO-001`.

## 2026-09-13 — Initialization reconciliation

### Fenwick HMG70ML-FS — eBay
**Status:** REJECTED / benchmark  
**Condition:** Pre-owned  
**Price:** $65 + $30 shipping = $95 delivered before tax  
**Configuration:** 7'0", Medium Light, Fast; appears 1-piece  
**Seller:** previously observed 100% positive feedback (233)  
**Deal Score:** ~7/10

Assessment: interesting rod at the headline price, but shipping moves acquisition to about $95. At that delivered price, a new Fenwick Eagle `EGLW70ML-FS-2` around $99.95 is highly competitive. At $65 local/no shipping, this would be materially more interesting.

### Fenwick HMG69ML-FS — eBay
**Status:** REJECTED / benchmark  
**Condition:** Pre-owned  
**Price:** $65 + $30 shipping  
**Configuration:** 6'9", Medium Light, Fast

Assessment: same seller/pricing structure as the HMG70ML-FS. Shipping substantially weakens the bargain.

### Fenwick HMG Carbon Veil 7' ML 2-piece — eBay
**Status:** REJECTED  
**Condition:** Pre-owned  
**Price:** $175 + $17.99 shipping ≈ $193 delivered before tax

Assessment: rare/interesting older model, but not a bargain at the observed delivered price.

### Fenwick HMGW72ML-FS-2 — retail reference
**Status:** BENCHMARK  
**Price:** about $179.95 new  
**Configuration:** 7'2", Medium Light, Fast, 2-piece, 1/8–5/8 oz

Assessment: current upscale HMG analogue to the Eagle reference configuration.

### Shimano Poison Adrena 172M — eBay / Tackle Berry
**Status:** OBSERVED / shipping-sensitive  
**Price:** previously observed around $174.47 used before shipping from Japan  
**Seller:** previously observed 100% positive feedback  
**Deal Score:** ~8/10 pending delivered cost

Assessment: potentially strong headline price, but international shipping materially controls whether it is actually a deal.

### Shimano 18 Poison Adrena 1611M+ — eBay
**Status:** SOLD/ENDED  
**Price:** previously observed $181.94 + $68.91 shipping ≈ $250.85  
**Deal Score:** previously ~8/10

Assessment: no longer actionable. Preserve as historical benchmark only.

### Shimano Crucial 7'11" MH swimbait rod — OfferUp
**Status:** STATUS UNKNOWN  
**Price:** previously observed around $75  
**Deal Score:** previously ~8.5/10 conditional on condition

Assessment: potentially genuine garage-find territory if still available and physically sound. Current status was not established during initialization.

### G. Loomis GLX 852C JWR — used market
**Status:** REJECTED / benchmark  
**Price:** previously observed about $299.95 plus shipping

Assessment: fair market example, not exceptional enough for this project's bargain goal.

### G. Loomis IMX-Pro 803C JWR — used market
**Status:** REJECTED / benchmark  
**Price:** previously observed about $230 + $20 shipping

Assessment: fair used-market pricing, not garage-find territory.

### Shimano Stradic FM ST1000HGFM — new-market benchmark
**Status:** BENCHMARK  
**Price:** previously observed about $202 shipped new  
**Deal Score:** ~8/10

Use as a practical benchmark; seek materially better opportunities.

### Shimano Stradic FM ST2500HGFM — new-market benchmark
**Status:** BENCHMARK  
**Price:** previously observed around $200 new  
**Deal Score:** ~8.5/10

Use as a practical benchmark; seek materially better opportunities.

## Future entry format

For each notable item preserve, where known:
- observation date
- source and listing identity/link when available
- lifecycle status
- exact model/SKU confidence
- asking price
- shipping
- delivered price
- condition
- seller claim
- independently verified evidence
- market/reference value
- red flags
- Deal Score
- rationale
- prior observation/change history

Do not silently overwrite earlier observed prices/statuses when a listing changes; preserve the transition.
