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

- Source coverage still needs operational validation across repeated runs, especially Facebook Marketplace, OfferUp, Craigslist, Mercari, estate-sale sites, Goodwill sources, independent tackle shops, and pawn/liquidation sources.
- Listing history is currently sparse because prior searches were conversational rather than ledger-driven.

## Immediate continuation point

Run the next fishing-domain Deal_Watch search using `WATCHLIST.md`, `SOURCES.md`, and `DEAL_RULES.md` as authoritative instructions. For rods, search both the named priority targets and the current REQUIRED/PREFERRED/EXCLUDE property framework. Record notable findings and source coverage in `LISTINGS.md`, then reconcile any durable rule or watchlist changes.

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
