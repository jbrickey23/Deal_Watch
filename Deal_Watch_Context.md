# Deal_Watch — Context

## Current authoritative state

`Deal_Watch` is a GitHub-backed durable project. Repository: `JBrickey23/Deal_Watch`. GitHub is the durable source of truth; ChatGPT conversations are working sessions.

The project uses canonical `Project:Domain:WatchType` identifiers. Active watches are `Deal_Watch:Fishing:WorkerRod`, `Deal_Watch:Fishing:StradicReel`, and `Deal_Watch:Hat:SweatbandMachine`. The Fishing watches currently share a legacy ChatGPT condition-watch automation named `Deal Watch — Fishing`; that broad automation label is not a canonical watch key and should be renamed or split during automation cleanup. No `Hat:SweatbandMachine` automation is assumed. The repository remains authoritative for targets, source coverage, domain rules, listing history, tasks, and decisions.

## Purpose and scope

The project exists to find, verify, evaluate, and track unusually good deals using durable watchlists, source definitions, evaluation rules, and listing history. Fishing emphasizes older, discontinued, misidentified, or undervalued premium rods and reels. Hat:SweatbandMachine seeks purpose-built, convertible, and sleeper machines capable of sewing leather sweatbands into formed felt hats.

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
- `DEAL_RULES.md` — Fishing scoring, valuation, verification, and reporting rules.
- `LISTINGS.md` — Fishing listing/history ledger and benchmarks.
- `HAT_MACHINE_DEAL_RULES.md` — Hat:SweatbandMachine mission-fit, conversion, valuation, and reporting rules.
- `HAT_MACHINE_LISTINGS.md` — Hat:SweatbandMachine listing/history ledger and benchmarks.

## Active watch — Fishing:WorkerRod

### Rod discovery framework

Rod discovery is specification-driven as well as model-driven. Named targets receive priority, but they are not an exhaustive whitelist. `WATCHLIST.md` assigns properties behavioral levels (`REQUIRED`, `PREFERRED`, and `EXCLUDE`) and is authoritative for their current values.

Preferred rod brands:
- Shimano
- Fenwick
- G. Loomis

Current general rod-property summary:

**REQUIRED**
- Medium-Light or Medium power
- Fast or Extra Fast action

**PREFERRED**
- 6'5"–7'2" length
- 2-piece construction

**EXCLUDE**
- None currently defined

Searches should also surface unfamiliar or unlisted models when they satisfy required properties, avoid exclusions, credibly match the preferred specification/quality profile, and offer unusually strong value. Preferred properties improve relevance but do not act as hard exclusions.

### Named rod role — Worker

`Worker` is now a durable fishing-domain role/specification class for the likely **go-to light spinning rod**. It is intended to cover panfish and trout through finesse/general bass; heavier existing rods handle bigger lures, heavy cover, and larger-fish work.

Worker summary:
- spinning;
- Medium-Light strongly preferred;
- Fast preferred, Extra Fast acceptable;
- roughly 6'8"–7'2" preferred;
- **2-piece strongly preferred for transport**;
- should fish about 1/8 oz well, with useful performance below 1/8 desirable;
- upper useful range at least 3/8 oz and preferably 1/2–5/8 oz;
- approximately 4–10 or 6–12 lb line class;
- shorter rear handle preferred;
- continuous/full cork grip preferred;
- roughly 1000–2500 spinning-reel pairing;
- intended for panfish, trout, Ned/drop-shot, light jigs, small plastics/swimbaits/hardbaits, finesse bass, and general open-water/light-duty bass.

For Worker scoring, 2-piece construction carries more weight than in the general rod framework. Exceptional 1-piece rods can still be surfaced but must be flagged as a transport compromise.

Current Worker anchors:
- **Value baseline:** Fenwick Eagle Walleye `EGLW70ML-FS-2`, about $99.95 new.
- **Performance benchmark:** Fenwick HMG Walleye `HMGW72ML-FS-2`, about $179.95 new.
- Other Fenwick targets include `EGLW69ML-XFS-2`, `HMG69ML-FS-2`, and older/discontinued Eagle/HMG/Elite/Walleye/Inshore/general spinning rods that fit the Worker role.

See `WATCHLIST.md` for the authoritative full Worker definition and evaluation behavior.

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
- Worker-compatible current/prior Fenwick Walleye, Inshore, Eagle, HMG, Elite, and general spinning rods.

## Active watch — Fishing:StradicReel

### Shimano reels
- Stradic FM `ST1000HGFM`
- Stradic FM 2500-size models, especially `ST2500HGFM`

See `WATCHLIST.md` for authoritative target details.

## Active watch — Hat:SweatbandMachine

Hat:SweatbandMachine asks: **Can this machine sew a leather sweatband into a formed felt hat?**

It searches three acquisition tracks:
- **Native:** documented purpose-built sweatband machines.
- **Convertible:** machines with suitable fundamental geometry and a specific reasonable modification path.
- **Sleeper:** cheap, poorly identified older industrial machines whose photos/model plates reveal favorable geometry.

Priority investigation includes Singer 103W2, verified Singer 107 subclasses, ASM 1107-1, Juki LS-341-related cylinder-arm designs, Consew 227/227R-class machines, Adler 69-class machines, 441-style cylinder-arm machines, and comparable post-bed/off-the-arm/free-arm industrials. Inclusion is for investigation, not automatic qualification.

Every candidate receives the formed-hat rotation, crown/brim-junction reach, clearance, stitch/feed, material-control, slow-speed, modification-feasibility, parts, condition, and all-in-cost tests in `HAT_MACHINE_DEAL_RULES.md`.

Search base: ZIP 98053 / approximately 500 miles where supported, plus compelling shipping-capable national listings.

Known purpose-built benchmarks and the first run are preserved in `HAT_MACHINE_LISTINGS.md`. The Juki MB-372/Z002 is a confirmed negative example.

## Current operating rules

- Maintain naming consistency: canonical project name is `Deal_Watch`; descriptive domain labels must not silently become project names.
- Use the canonical keys `Fishing:WorkerRod`, `Fishing:StradicReel`, and `Hat:SweatbandMachine`; domain-only or item-only labels are shorthand, not watch identities.
- Label Fishing ledger entries as `Fishing:WorkerRod` or `Fishing:StradicReel` within `LISTINGS.md`; use `HAT_MACHINE_DEAL_RULES.md` / `HAT_MACHINE_LISTINGS.md` only for `Hat:SweatbandMachine`.
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

- Fenwick Eagle `EGLW70ML-FS-2`: 7'0", Medium Light, Fast, 2-piece, 1/8–5/8 oz, 4–10 lb line; reference new price about $99.95. Worker value baseline.
- Fenwick HMG `HMGW72ML-FS-2`: 7'2", Medium Light, Fast, 2-piece, 1/8–5/8 oz; reference new price about $179.95. Current Worker performance benchmark.
- Shimano Stradic FM `ST1000HGFM`: reference MSRP/direct price about $234.99.
- Shimano Stradic FM `ST2500HGFM`: reference MSRP/direct price about $254.99.

These are working benchmarks, not permanent truths. Re-verify current manufacturer/retail data when materially relevant.

## Current automation state

A daily condition-watch automation with the legacy broad name `Deal Watch — Fishing` is enabled for the Fishing watch keys. It is an execution mechanism; the repository's current `WATCHLIST.md`, rules, and durable decisions are authoritative when execution wording and repository state differ.

## Open issues

- Source coverage still needs operational validation across repeated runs, especially Facebook Marketplace, OfferUp, Craigslist, Mercari, estate-sale sites beyond BidRush, Goodwill sources, independent tackle shops, and pawn/liquidation sources.
- BidRush direct item pages and site search have been validated as readable from ChatGPT/workspace tooling, but future runs should continue testing search quality because results can be fuzzy/noisy.
- Listing history is currently sparse because prior searches were conversational rather than ledger-driven.
- Worker research should continue opportunistically across older/discontinued Fenwick generations and later across other manufacturers, but the role definition is stable enough for Fishing execution.
- Hat:SweatbandMachine source coverage needs repeated validation across the newly added industrial dealers, upholstery/leather/canvas channels, liquidations, and poorly identified local industrial machines.

## Immediate continuation point

The current continuation focus is **`Deal_Watch:Hat:SweatbandMachine`**. Run the next Hat:SweatbandMachine search using the `Domain — Hat:SweatbandMachine` section of `WATCHLIST.md`, the Hat-specific sources and adjacent-trade searches in `SOURCES.md`, `HAT_MACHINE_DEAL_RULES.md`, and `HAT_MACHINE_LISTINGS.md`.

Search both exact-purpose models and broad architecture/sleeper listings. Apply the formed-hat geometry and specific conversion-feasibility test before assigning mission fit. Record meaningful findings and actual source coverage in `HAT_MACHINE_LISTINGS.md`.

`Deal_Watch:Fishing:WorkerRod` and `Deal_Watch:Fishing:StradicReel` remain active and may be run separately using `DEAL_RULES.md` and `LISTINGS.md`. Do not combine the two domain ledgers.

## Restore order for a new chat

1. `README.md`
2. `Deal_Watch_Context.md`
3. `Deal_Watch_TODO.md`
4. `Deal_Watch_Decision_Log.md`
5. `WATCHLIST.md`
6. `SOURCES.md`
7. `DEAL_RULES.md`
8. `LISTINGS.md`
9. `HAT_MACHINE_DEAL_RULES.md`
10. `HAT_MACHINE_LISTINGS.md`
11. `Deal_Watch_New_Chat_Bootstrap_Prompt.md`

Always use the latest repository state rather than prior chat memory when they conflict.

## Reconciled chat additions — 2026-09-15 — Worker research

A focused Fenwick comparison established the `Worker` role. The research compared current and prior Fenwick Eagle, HMG, Elite, Walleye, Bass, and Inshore configurations. The durable conclusion is not that a single Fenwick SKU is permanently selected, but that `HMGW72ML-FS-2` is the current new-rod performance benchmark and `EGLW70ML-FS-2` is the value baseline.

Important user-use constraints established during the research:
- 2-piece construction is strongly preferred for ease of transport;
- shorter handle geometry is preferred;
- continuous/full cork is preferred;
- the Worker should complement existing heavier rods rather than duplicate them;
- the useful mission is panfish/trout through finesse and general light-duty bass;
- older Marketplace rods with similar specifications are desirable when they beat the current new benchmarks on price/performance.

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
