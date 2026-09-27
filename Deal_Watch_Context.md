# Deal_Watch — Context

## Session handoff — 2026-09-26 inventory and hat steamer

The current fishing work is `Deal_Watch:FishingInventory`. `FISHING_INVENTORY.md` is authoritative for owned gear. Reconciled 2026-09-26 confirmations: Ugly Stik GX2 spinning `USGXSP662M` = 6'6", Medium power, 2-piece, 6–15 lb, 1/8–5/8 oz; current manufacturer data leaves conventional action unspecified, while the physical rod's `Action: Medium` stamp is retained as a known labeling inconsistency. Ugly Stik GX2 casting `USGXCAP561M` = 5'6", Medium power, 1-piece, 8–20 lb, 1/4–5/8 oz, with the same physical `Action: Medium` labeling issue. DreamCatcher spinning `Z201` = 6'6", Medium, Fast, 3/16–2 oz, 8–20 lb; applicability of those ratings across its previously reported M/MH tips remains open. South Bend Elite `ES-323A` physical markings are confirmed: 5'6", 2-piece, Light, 4–8 lb, 1/8–3/8 oz. Shimano Spirex is exact-model confirmed `SR1000FG`; Shimano specs are 6.2:1, 7 lb max drag, 8.8 oz, 28 in/turn, 5+1 bearings, mono 2/270, 4/140, 6/110. Lew's Classic Pro Speed Spool SLP is exact-model confirmed `CP1SHL`, left-hand. Pflueger President is physically verified `PRES20`, explicitly NOT `PRES20X`; older PRES20-specific specs remain to verify. Continue resolving DreamCatcher CARBONITE specs, PRES20 specs, actual rod/reel pairings, additional owned gear, and ultimately the Fenwick Eagle `EGLW66M-FS-2` keep/return decision.

The user also compared steamers for shaping/blocking felt hats. A pictured, seller-described Jiffy J-2000 Limited Edition missing an upright wand holder was offered used for $200; a $100 offer was contemplated, but no purchase was reported. Another pictured white/gray hose steamer could not be identified reliably by photo; do not label it Jiffy without its model plate. The user favored a purpose-built hat steamer to reduce repair/compatibility uncertainty and found a new Jiffy J-2000H at $165 plus estimated $26.19 shipping ($191.19 estimated total, final shipping subject to approval if higher). The cart is a price comparison, **not a confirmed order**. This hat-shaping steamer discussion is distinct from the active `Hat:SweatbandMachine` watch, which concerns sewing sweatbands. Do not silently create a steamer watch or record the steamer as owned.

## Current authoritative state

`Deal_Watch` is a GitHub-backed durable project. Repository: `JBrickey23/Deal_Watch`. GitHub is the durable source of truth; ChatGPT conversations are working sessions.

The project uses canonical `Project:Domain:WatchType` identifiers. Active watches are `Deal_Watch:Fishing:WorkerRod`, `Deal_Watch:Fishing:StradicReel`, and `Deal_Watch:Hat:SweatbandMachine`. The Fishing watch state changed on 2026-09-26: the user has procured the Fenwick HMG Walleye `HMGW72ML-FS-2` Worker benchmark and a Stradic 1000HG / `ST1000HGFM`-class reel. The other received Fenwick is now identified as `EGLW66M-FS-2`, a 6'6" Medium Fast 2-piece Eagle Walleye rated 6-12 lb and 1/8-3/4 oz. Future fishing searches should avoid ordinary duplicates and instead focus on materially different lineup slots, exceptional backup pricing, and evaluation of whether the `EGLW66M-FS-2` is distinct enough from the HMG Worker to keep. The Fishing watches currently share a legacy ChatGPT condition-watch automation named `Deal Watch — Fishing`; that broad automation label is not a canonical watch key and should be renamed or split during automation cleanup. No `Hat:SweatbandMachine` automation is assumed. The repository remains authoritative for targets, source coverage, domain rules, listing history, tasks, and decisions.

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

GitHub write access has been verified for both normal text updates and binary assets. For ordinary UTF-8 files, use `fetch_file` plus `update_file` / `create_file`. For binary assets such as reel images, use the Git object path: `create_blob` with base64 content, `create_tree`, `create_commit`, and `update_ref`. Do not assume binary upload is unavailable merely because the simple UTF-8 contents wrapper is exposed first.

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
- **Owned Worker benchmark:** Fenwick HMG Walleye `HMGW72ML-FS-2`.
- **Value baseline / overlap comparison:** Fenwick Eagle Walleye `EGLW70ML-FS-2`, about $99.95 new.
- **Pending lineup decision:** Fenwick Eagle Walleye `EGLW66M-FS-2` should be evaluated as a possible shorter/heavier utility rod: 6'6", Medium, Fast, 2-piece, 6-12 lb, 1/8-3/4 oz. It is likely distinct from the owned HMG Worker on length/power/upper lure range, but may still overlap depending on the user's existing rod lineup.
- Other Fenwick targets such as `EGLW69ML-XFS-2`, `HMG69ML-FS-2`, and older/discontinued Eagle/HMG/Elite/Walleye/Inshore/general spinning rods remain useful only when they fill a distinct role or are true bargain/backup opportunities.

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
- **Procured:** Stradic 1000HG / `ST1000HGFM`-class reel; ordinary duplicate 1000-size listings should no longer alert.
- Continue watching Stradic FM 2500-size models, especially `ST2500HGFM`, when they fill a distinct role or materially beat ordinary new-market pricing.

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
- Use GitHub as the durable write path. Text-file updates can use the contents wrapper; binary assets must use Git blobs/trees/commits and fast-forward the branch ref.
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

The current continuation focus is **Fishing lineup reconciliation plus `Deal_Watch:Hat:SweatbandMachine`**. First resolve `DW-TODO-011` by itemizing owned fishing gear, then use that inventory to resolve `DW-TODO-010`: decide whether the received Fenwick Eagle Walleye `EGLW66M-FS-2` replaces an existing rod, fills a distinct shorter/heavier utility slot, or overlaps too closely with the owned `HMGW72ML-FS-2`. Run the next Hat:SweatbandMachine search using the `Domain — Hat:SweatbandMachine` section of `WATCHLIST.md`, the Hat-specific sources and adjacent-trade searches in `SOURCES.md`, `HAT_MACHINE_DEAL_RULES.md`, and `HAT_MACHINE_LISTINGS.md`.

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
11. `REEL_IMAGES.md`
12. `FISHING_INVENTORY.md`
13. `Deal_Watch_New_Chat_Bootstrap_Prompt.md`

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
