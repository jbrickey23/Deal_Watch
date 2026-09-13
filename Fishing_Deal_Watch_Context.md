# Fishing Deal Watch — Context

## Current authoritative state

Fishing Deal Watch is initialized as a GitHub-backed durable project. GitHub is the durable source of truth; ChatGPT conversations are working sessions.

An existing ChatGPT automation named `Fishing Deal Watch` is enabled and runs daily as a condition watch. It currently searches for the target gear defined in this repository, but the repository—not the automation prompt—should become the authoritative source for watch targets, source coverage, deal rules, and listing history.

## Purpose and scope

The project exists to find, verify, and evaluate unusually good fishing-gear deals, especially older, discontinued, misidentified, or undervalued premium rods and reels.

Primary goals:
- find genuine bargain listings rather than merely fair retail prices;
- identify exact models and generations where possible;
- distinguish seller claims from what can actually be verified from text/photos;
- include delivered cost, condition, transaction risk, and realistic market value;
- preserve listing history so already-reviewed items are not repeatedly rediscovered from scratch;
- make source coverage explicit so `nothing found` is distinguishable from `not searched` or `inaccessible`.

## Durable records

- `Fishing_Deal_Watch_Context.md` — current project state and continuation point.
- `Fishing_Deal_Watch_TODO.md` — unfinished durable work.
- `Fishing_Deal_Watch_Decision_Log.md` — durable decisions and operating rules.
- `Fishing_Deal_Watch_New_Chat_Bootstrap_Prompt.md` — fresh-chat restoration instructions.
- `WATCHLIST.md` — authoritative target gear and configurations.
- `SOURCES.md` — source checklist and coverage expectations.
- `DEAL_RULES.md` — scoring, valuation, verification, and reporting rules.
- `LISTINGS.md` — known listing/history ledger and benchmark observations.

## Current target categories

### Shimano rods
- Expride
- Zodias
- Cumara
- Crucial
- Poison Adrena

### G. Loomis rods
Comparable premium Loomis rods are in scope, including GLX, IMX, IMX-Pro, NRX and related models when value is compelling.

### Fenwick rods
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

A ChatGPT daily condition-watch automation named `Fishing Deal Watch` exists and is enabled. Its current prompt predates this repository and contains much of the current watchlist directly. A future improvement is to make automation behavior align explicitly with the durable repository records so the prompt does not become a competing source of truth.

## Open issues

- Source coverage still needs operational validation across repeated runs, especially Facebook Marketplace, OfferUp, Craigslist, Mercari, estate-sale sites, Goodwill sources, independent tackle shops, and pawn/liquidation sources.
- Listing history is currently sparse because prior searches were conversational rather than ledger-driven.
- The automation does not yet explicitly report its source-coverage footer or read from these durable records.

## Immediate continuation point

Run the next Fishing Deal Watch search using `WATCHLIST.md`, `SOURCES.md`, and `DEAL_RULES.md` as the authoritative instructions. Record notable findings and source coverage in `LISTINGS.md`, then reconcile any durable rule or watchlist changes.

## Restore order for a new chat

1. `README.md`
2. `Fishing_Deal_Watch_Context.md`
3. `Fishing_Deal_Watch_TODO.md`
4. `Fishing_Deal_Watch_Decision_Log.md`
5. `WATCHLIST.md`
6. `SOURCES.md`
7. `DEAL_RULES.md`
8. `LISTINGS.md`
9. `Fishing_Deal_Watch_New_Chat_Bootstrap_Prompt.md`

Always use the latest repository state rather than prior chat memory when they conflict.
