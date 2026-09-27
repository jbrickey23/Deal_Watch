# Deal_Watch — Fishing Watch Rules

This file defines shared evaluation behavior for `Deal_Watch:Fishing:WorkerRod` and `Deal_Watch:Fishing:StradicReel`. Every reported listing must identify which watch key applies.

## Deal Score

Use a 1–10 scale based on acquisition value, not product quality alone.

- **10 — Exceptional / buy immediately**
- **9 — Rare bargain**
- **8 — Strong buy**
- **7 — Interesting**
- **6 — Fair market**
- **Below 6 — Usually do not surface unless unusual or strategically informative**

## Core evaluation factors

Evaluate:
- asking price
- shipping and other unavoidable acquisition costs
- delivered price before tax where tax cannot be known precisely
- exact model/SKU confidence
- generation/year confidence
- visible condition
- seller description versus photographic evidence
- realistic used/new value
- seller feedback/reputation
- return policy or transaction risk
- local-pickup advantage where relevant
- rarity or discontinued status
- misidentification/mispricing potential

## Price discipline

Shipping counts. A $65 rod plus $30 shipping is a $95 acquisition before tax, not a $65 deal.

Reference retail prices are baselines, not deal scores. Current/new equivalents should be checked when a used price approaches new pricing.

Do not reward a listing simply because the product itself is premium.

## Misidentified listings

A listing can become more interesting when:
- seller title is generic or wrong;
- exact model is visible in photos;
- photos indicate a higher-value generation/model than the description suggests;
- bundled gear obscures a valuable component.

Do not convert suspicion into certainty. Report confidence and what evidence supports identification.

## Rod inspection checklist

Flag:
- blank cracks, impact marks, repairs, or suspicious finish changes
- guide-frame bending or missing/chipped inserts
- ferrule fit/wear on multi-piece rods
- reel-seat damage or looseness
- altered/replaced grips or handles
- shortened tips
- mismatched sections
- seller description inconsistent with model markings

## Reel inspection checklist

Flag:
- exact SKU uncertainty
- spool-lip nicks/damage
- handle wear or looseness
- bail damage/misalignment
- corrosion or likely saltwater abuse
- abnormal cosmetic wear
- missing box, handle, spool, washers, or accessories
- weak seller history or restrictive/no-return terms

## Reporting format

For worthwhile listings, report:
- listing/source
- asking price
- shipping
- delivered price
- exact model/SKU if identifiable
- seller claim
- what is independently verified
- likely market/reference value
- notable risks/red flags
- Deal Score 1–10
- concise category: `fair price`, `interesting`, `strong buy`, or `grab it`

## Post-procurement fishing filters

Because the Fenwick HMG Walleye `HMGW72ML-FS-2` and a Stradic 1000HG have been procured, future Fishing notifications should not alert on ordinary duplicates of those exact roles.

Surface additional HMGW72ML-FS-2 / Worker-like rods only when:
- the price is true backup/flip territory;
- condition is excellent and delivered cost materially beats current owned/new benchmarks;
- the rod fills a demonstrably different slot from the owned HMG Worker; or
- the listing helps evaluate whether the user's other received Fenwick should replace an existing rod.

Surface additional Stradic 1000HG listings only when they are exceptional backup/spare-value opportunities. For a next primary reel, prioritize compact-body C2000/C2500-class designs, including JDM-only or JDM-first variants, that retain roughly 1000-size body feel while adding useful spool diameter/capacity/retrieve. Favor 43–44 mm spools, approximately 150–185 g class weight where model-appropriate, shallow spools suitable for braid-to-leader/light mono/fluoro, and 5–8 lb mono / PE 0.6–1.0-class capacity. Include Shimano Stradic, Vanford, Twin Power, Vanquish and comparable Daiwa Caldia/Luvias compact FC/LT variants. Treat ordinary full-size 2500/3000 reels as lower-priority because the user finds them too large; surface them only when they are unusually light/compact, exceptionally priced, or fill a clearly distinct role.

## Notification threshold

The legacy automation executing the Fishing watch keys should notify only for worthwhile **new** or **meaningfully changed** listings.

Meaningful changes include:
- new listing
- material price drop
- new evidence that changes model identification or condition confidence
- availability/status change that makes an otherwise interesting listing actionable

Do not notify merely because an unchanged fair-market listing still exists.

## Known working thresholds

### Fenwick Eagle EGLW70ML-FS-2
Reference new price: about $99.95.
- used around $60 or less: potentially strong
- genuinely new around ~$75: attractive
- used around ~$95 delivered: generally weak versus new

### Fenwick HMGW72ML-FS-2
Reference new price: about $179.95.
- ~$90–110 excellent condition: interesting
- under $80: strong buy
- ~$60–70: grab-it territory if clean and verified

### Shimano Stradic FM ST1000HGFM
Reference MSRP/direct: about $234.99.
- ~$202 shipped new has previously benchmarked around 8/10
- seek meaningfully better pricing or unusual value

### Shimano Stradic FM ST2500HGFM
Reference MSRP/direct: about $254.99.
- around $200 new has previously benchmarked around 8.5/10 on price alone
- user ergonomics now reduce its strategic priority because conventional 2500-size reels feel too large
- surface only at unusually strong value or when weight/fit makes it competitive with compact-body alternatives

These thresholds are provisional and should evolve from observed market evidence under legacy task `FDW-TODO-004`.
