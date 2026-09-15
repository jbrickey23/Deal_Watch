# Deal_Watch — Context

## Current authoritative state

`Deal_Watch` is a GitHub-backed durable project. Repository: `JBrickey23/Deal_Watch`. GitHub is the durable source of truth; ChatGPT conversations are working sessions.

The project is domain-agnostic by design. **Fishing** is the current watch domain. An enabled ChatGPT condition-watch automation named `Deal Watch — Fishing` executes that domain watch; the repository remains authoritative for targets, source coverage, deal rules, listing history, tasks, and decisions.

## Purpose and scope

The project exists to find, verify, evaluate, and track unusually good deals using durable watchlists, source definitions, evaluation rules, and listing history. The current fishing domain emphasizes older, discontinued, misidentified, or undervalued premium rods and reels.

Primary goals:
- find genuine bargains rather than merely fair retail prices;
- identify exact models and generations where possible;
- distinguish seller claims from what can actually be verified from text/photos;
- include delivered cost, condition, transaction risk, and realistic market value;
- preserve listing history so already-reviewed items are not repeatedly rediscovered from scratch;
- make source coverage explicit so `nothing found` is distinguishable from `not searched` or `inaccessible`.

## Durable records

- `Deal_Watch_Context.md` — current project state and continuation point.
- `Deal_Watch_TODO.md` — unfinished durable work.
- `Deal_Watch_Decision_Log.md` — durable decisions and operating rules.
- `Deal_Watch_New_Chat_Bootstrap_Prompt.md` — fresh-chat restoration instructions.
- `WATCHLIST.md` — authoritative targets and configurations for the current watch domain.
- `SOURCES.md` — source checklist and coverage expectations.
- `DEAL_RULES.md` — scoring, valuation, verification, and reporting rules.
- `LISTINGS.md` — known listing/history ledger and benchmark observations.

## Current watch domain — Fishing

### Rod discovery framework

Rod discovery is specification-driven as well as model-driven. Named targets receive priority, but they are not an exhaustive whitelist. `WATCHLIST.md` assigns properties behavioral levels (`REQUIRED`, `PREFERRED`, and `EXCLUDE`) and is authoritative for their current values.

Preferred rod brands:
- Shimano
- Fenwick
- G. Loomis

Current rod-property summary:

**REQUIRED**
- Medium-Light or Medium power
- Fast or Extra Fast action

**PREFERRED**
- 6'5"–7'2" length
- 2-piece construction

**EXCLUDE**
- None currently defined

Searches should also surface unfamiliar or unlisted models when they satisfy required properties, avoid exclusions, credibly match the preferred specification/quality profile, and offer unusually strong value. Preferred properties improve relevance but do not act as hard exclusions.

### Shimano rods — named priority targets
- Expride
- Zodias
- Cumara
- Crucial
- Poison Adrena

### G. Loomis rods — named priority targets
Comparable premium Loomis rods are in scope, including GLX, IMX, IMX-Pro, NRX and related models when value is compelling. Also search beyond those named families when specifications, quality, and value fit.

### Fenwick rods — named priority targets
- Eagle `EGLW70ML-FS-2`
- HMG-family rods near the Eagle reference configuration, especially:
  - `HMGW72ML-FS-2`
  - `HMG69ML-FS-2`
  - `HMG70ML-FS`
  - similar discontinued HMG variants

### Shimano reels
- Stradic FM `ST1000HGFM`
- Stradic FM 2500-size models, especially `ST2500HGFM`

See `WATCHLIST.md` for authoritative target details.

## Current operating rules

- Maintain naming consistency: canonical project name is `Deal_Watch`; descriptive domain labels must not silently become project names.
- Use `Fishing` as the current watch-domain label, not as the canonical project name.
- Preserve existing `FDW-*` task and decision IDs as stable historical identifiers. New durable IDs use the `DW-*` prefix.
- Treat ChatGPT conversations as working sessions. Before deleting an old chat, reconcile any important decisions, actions, listings, source findings, rule changes, or continuation details into the GitHub repository.
- Rod searches must combine current watch-property levels and preferred qualities with named priority targets rather than treating named models as an exhaustive whitelist.
- `WATCHLIST.md` is authoritative for current property assignments; context and decision records should describe semantics without overriding newer watchlist values.
- Delivered price matters more than headline price.
- Exact model/SKU should be verified where possible.
- A mislabeled listing may be more interesting, not less, if photos indicate a better item than the seller realizes.
- Do not imply a source was searched when it was not actually searched.
- Run reports should distinguish `SEARCHED`, `INACCESSIBLE`, and `NOT SEARCHED` source states.
- Track listing lifecycle states such as `NEW`, `PRICE DROP`, `STILL AVAILABLE`, `SOLD/ENDED`, and `REJECTED`.
- Deal scores are 1–10 and should reflect actual acquisition value, not product quality alone.
- Fair-market listings should generally not trigger notifications unless they are otherwise unusual.

## Known price/configuration anchors

- Fenwick Eagle `EGLW70ML-FS-2`: 7'0", Medium Light, Fast, 2-piece, 1/8–5/8 oz, 4–10 lb line; reference new price about $99.95.
- Fenwick HMG `HMGW72ML-FS-2`: 7'2", Medium Light, Fast, 2-piece, 1/8–5/8 oz; reference new price about $179.95.
- Shimano Stradic FM `ST1000HGFM`: reference MSRP/direct price about $234.99.
- Shimano Stradic FM `ST2500HGFM`: reference MSRP/direct price about $254.99.

These are working benchmarks, not permanent truths. Re-verify current manufacturer/retail data when materially relevant.

## Current automation state

A daily condition-watch automation named `Deal Watch — Fishing` is enabled for the fishing domain. It is an execution mechanism; the repository's current `WATCHLIST.md`, rules, and durable decisions are authoritative when execution wording and repository state differ.

## Open issues

- Source coverage still needs operational validation across repeated runs, especially Facebook Marketplace, OfferUp, Craigslist, Mercari, estate-sale sites beyond BidRush, Goodwill sources, independent tackle shops, and pawn/liquidation sources.
- BidRush direct item pages and site search have been validated as readable from ChatGPT/workspace tooling, but future runs should continue testing search quality because results can be fuzzy/noisy.
- Listing history is currently sparse because prior searches were conversational rather than ledger-driven.

## Immediate continuation point

Run the next fishing-domain Deal_Watch search using `WATCHLIST.md`, `SOURCES.md`, and `DEAL_RULES.md` as authoritative instructions. For rods, search both the named priority targets and the current REQUIRED/PREFERRED/EXCLUDE property framework. Record notable findings and source coverage in `LISTINGS.md`, then reconcile any durable rule or watchlist changes.

Specific current follow-up from the 2026-09-15 BidRush-only run: two active pickup-only Port Ludlow mixed fishing lots are preserved in `LISTINGS.md` and may merit deeper photo inspection before their 2026-09-17 UTC close if the user wants to pursue local estate-lot upside.

## Restore order for a new chat

1. `README.md`
2. `Deal_Watch_Context.md`
3. `Deal_Watch_TODO.md`
4. `Deal_Watch_Decision_Log.md`
5. `WATCHLIST.md`
6. `SOURCES.md`
7. `DEAL_RULES.md`
8. `LISTINGS.md`
9. `Deal_Watch_New_Chat_Bootstrap_Prompt.md`

Always use the latest repository state rather than prior chat memory when they conflict.

## Reconciled chat additions — 2026-09-14

### Facebook Marketplace access and links

Authenticated Facebook Marketplace access was successfully established in a prior Work browser session. The verified search scope was Redmond/98053 represented by Facebook as Ames Lake, within 500 miles. Marketplace entries should preserve full stable item URLs in this format:

`https://www.facebook.com/marketplace/item/<listing_id>/`

The latest ledger entries in `LISTINGS.md` preserve clickable Marketplace URLs. If the Work browser environment is unavailable in a future run, mark authenticated Facebook Marketplace as `INACCESSIBLE` or `NOT SEARCHED AUTHENTICATED` rather than treating public indexed results as native Marketplace coverage.

### Possible future watch domain — Felt hats

A possible future Deal_Watch domain was discussed but not activated. Fishing remains the current active watch domain unless the user explicitly requests a domain switch.

The proposed felt-hat domain focuses on thrift, garage-sale, and estate-sale hat buys that can be reshaped/upcycled. Key evaluation dimensions:
- material: rabbit felt, beaver felt, beaver blend, 50/50 beaver/rabbit, credible fur felt;
- size: larger sizes generally improve utility/resale/upcycle value;
- condition: structurally usable felt body, reshape potential, sweatband/liner/tag condition, no severe moth damage, rot, mold, oil saturation, or structural collapse;
- price: under $100 is a broad first-pass interesting range for verified quality felt, with price/value thresholds to be refined from observed data.

Hat-material signals should be treated by confidence:
- HIGH: visible tag/sweatband/liner states `100% beaver`, `pure beaver`, `50/50 beaver/rabbit`, `beaver blend`, or `fur felt`;
- MEDIUM: reputable brand plus X/XXX rating or known quality line consistent with the brand/era;
- LOW: seller claim without photos of markings;
- REJECT or practice-only: wool felt, crushable wool, costume hats, severe damage, or unclear material at high price.

X ratings are useful signals but not standardized across brands or eras. Do not assume a fixed beaver percentage from `3X`, `5X`, `10X`, `XXX`, `50X`, etc. Exact material markings such as `50/50 beaver/rabbit` carry more evidentiary weight than X-count alone.

Visual verification workflow for hats should inspect:
1. listing title, price, location, and full URL;
2. all visible text and image captions;
3. photos for brand, size, felt/material markings, X rating, sweatband, liner, brim edge, crown shape, moth holes, cracks, oil/sweat staining, water damage, and reshapeable structure;
4. material confidence: HIGH / MEDIUM / LOW / REJECT;
5. condition confidence: USABLE / QUESTIONABLE / REJECT;
6. price/value tier;
7. next action: ALERT / NEEDS SELLER QUESTIONS / WATCH / BENCHMARK / REJECT.

Seller follow-up for hat verification should ask for close-up photos of the inside sweatband markings, size tag, liner/logo, brim edge, and any damage/moth holes, plus whether the hat says fur felt, beaver, rabbit, wool, or any X rating.
