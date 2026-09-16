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
- around $200 new has previously benchmarked around 8.5/10
- seek meaningfully better pricing or unusual value

These thresholds are provisional and should evolve from observed market evidence under legacy task `FDW-TODO-004`.
