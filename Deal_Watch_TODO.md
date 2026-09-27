# Deal_Watch — TODO

Canonical list of unfinished, blocked, waiting, or deferred work. IDs are never reused.

Legacy `FDW-*` IDs are preserved as stable historical identifiers. New task IDs use the `DW-*` prefix.

## OPEN

### DW-TODO-011 — Itemize owned fishing gear
**Priority:** High  
**Status:** OPEN / IN PROGRESS

2026-09-26 checkpoint: owned fishing inventory is now substantially reconciled. Confirmed pairings are HMG `HMGW72ML-FS-2` + Stradic 1000HG, Ugly Stik GX2 spinning `USGXSP662M` + Shimano Spirex `SR1000FG`, DreamCatcher `Z201` + Shimano IX 2000, South Bend Elite `ES-323A` + Pflueger President `PRES20`, and Ugly Stik GX2 casting `USGXCAP561M` + Lew's `CP1SHL`. A JDM Shimano 23 Stradic `C2500S` (UPC `4969363045805`, 5.1:1, 6 ball bearings, Malaysia origin) has been ordered and is in transit for the Fenwick Eagle `EGLW66M-FS-2`. Reel strategy now favors compact-body JDM C2000/C2500-style reels over conventional full-size 2500/3000 reels because the user prefers 1000-class body feel. Remaining inventory work centers on DreamCatcher CARBONITE specs/pairing, Z201 two-tip rating applicability, older PRES20-specific specs/condition, any additional owned gear, and final keep/replace role assignments.

Create a durable inventory of the user's owned fishing rods and reels so Deal_Watch can evaluate lineup gaps, overlap, replacement candidates, and future search targets against actual owned gear instead of isolated deals.

Success criteria:
- list owned rods with maker/model, length, power, action, piece count, lure rating, line rating, handle notes, intended role, and keep/replace/unknown status;
- list owned reels with maker/model/SKU/generation, size, intended pairing, condition, and keep/replace/unknown status;
- identify current lineup roles and gaps;
- use the inventory to resolve `DW-TODO-010` for `EGLW66M-FS-2`;
- update Fishing search parameters so future alerts fill gaps rather than duplicate owned gear.

### DW-TODO-007 — Define felt-hat domain if user switches from fishing
**Priority:** Medium  
**Status:** OPEN

If the user decides to switch Deal_Watch from fishing to hats, create/reconcile a hat-domain watchlist and deal rules before running the new domain.

Initial hat-domain focus:
- thrift, garage-sale, estate-sale, and under-described listings;
- reshape/upcycle candidates rather than generic fashion hats;
- rabbit felt, beaver felt, beaver blend, 50/50 beaver/rabbit, or credible fur felt;
- size, condition, price, and visual verification of markings;
- X/XXX ratings as non-standard quality clues, not fixed material percentages.

Success criteria:
- `WATCHLIST.md` rewritten or extended for the hat domain;
- `DEAL_RULES.md` includes hat material-confidence, condition-confidence, and price/value thresholds;
- `SOURCES.md` reflects hat-appropriate source terms and marketplaces;
- `LISTINGS.md` records hat listings with full clickable URLs and material/condition evidence.

### DW-TODO-006 — Verify ChatGPT Project Instructions after canonical rename
**Priority:** High  
**Status:** OPEN

Verify that the ChatGPT Project named `Deal_Watch` uses the canonical repository `JBrickey23/Deal_Watch` and the renamed durable files (`Deal_Watch_Context.md`, `Deal_Watch_TODO.md`, `Deal_Watch_Decision_Log.md`, and `Deal_Watch_New_Chat_Bootstrap_Prompt.md`). Remove any stale `Fishing_Deal_Watch`, `Fishing Deal Watch`, or `Deal_Watcher` references that incorrectly identify the project rather than the fishing watch domain.

Success criteria:
- ChatGPT Project name is `Deal_Watch`;
- Project Instructions reference `JBrickey23/Deal_Watch`;
- restore/reconcile instructions use the canonical `Deal_Watch_*` filenames;
- canonical watch identifiers use `Project:Domain:WatchType`;
- replace or split the legacy automation label `Deal Watch — Fishing` so automation execution maps visibly to `Fishing:WorkerRod` and `Fishing:StradicReel`.

### FDW-TODO-001 — Validate source coverage across real runs
**Priority:** High  
**Status:** OPEN

Run the fishing-domain watch repeatedly using the source checklist in `SOURCES.md` and determine which sources are reliably searchable, intermittently searchable, login-limited, or effectively inaccessible from ChatGPT.

Success criteria:
- coverage status is known for every primary source;
- reports distinguish `SEARCHED`, `INACCESSIBLE`, and `NOT SEARCHED`;
- source rules are updated from evidence rather than assumptions.

### FDW-TODO-003 — Establish listing-history discipline
**Priority:** Medium  
**Status:** OPEN

Use `LISTINGS.md` on future runs to preserve known listings, prior prices, status changes, rejections, and rationale. Avoid repeatedly re-evaluating unchanged listings as though they were new.

### FDW-TODO-004 — Refine deal thresholds from observed market data
**Priority:** Medium  
**Status:** OPEN

As more listings are evaluated, update `DEAL_RULES.md` with evidence-backed thresholds for target rods/reels. Preserve the distinction between reference retail, ordinary used market, and true bargain pricing.

### FDW-TODO-005 — Evaluate whether lightweight software adds value
**Priority:** Low  
**Status:** DEFERRED

After roughly 10–20 durable search runs, assess whether code, GitHub Actions, structured collectors, or another automated pipeline would materially improve discovery, deduplication, price-history tracking, or source coverage. Do not build software merely because the project is durable.

## DONE

### DW-TODO-010 — Evaluate Fenwick EGLW66M-FS-2 before return
**Priority:** High
**Status:** DONE — KEEP (2026-09-27; see DW-DEC-019)

The 6'6" Medium Fast Eagle (6–12 lb, 1/8–3/4 oz) is the primary compact Medium spinning rod with the incoming 23 Stradic `C2500S`. The 7'2" Medium Light Fast HMG and Stradic 1000HG remain the light Worker pair. The 6'6" Medium GX2 spinning `USGXSP662M` (6–15 lb, 1/8–5/8 oz) overlaps the Eagle most closely and moves to backup/loaner/rough-duty service with its Spirex `SR1000FG`; no disposal decision is implied. Rod action on the GX2 remains unspecified in manufacturer data despite its `Action: Medium` stamp. The return deadline was not supplied or recorded and is unknown; this recommendation is based on the documented lineup, before an on-water test or hands-on balance check with the incoming reel. Fishing watch targets were narrowed to avoid ordinary duplicates of both filled roles.


### DW-TODO-012 — Mirror reel image binaries into GitHub
**Priority:** Medium  
**Status:** DONE

Mirrored current reel reference images into GitHub under `assets/reels/` and updated `REEL_IMAGES.md` plus `FISHING_INVENTORY.md` to use repository-hosted image paths while preserving source attribution.

### DW-TODO-009 — Adopt qualified watch-key naming
**Priority:** High  
**Status:** DONE

Adopted `Project:Domain:WatchType` as the canonical naming grammar. Reconciled current watches as `Deal_Watch:Fishing:WorkerRod`, `Deal_Watch:Fishing:StradicReel`, and `Deal_Watch:Hat:SweatbandMachine`; updated operational files and preserved old broad labels only as historical shorthand.

### DW-TODO-008 — Reconcile active multi-domain state
**Priority:** High  
**Status:** DONE

Reconciled Fishing and Hat:Machine as simultaneous active domains. Added `HAT_MACHINE_DEAL_RULES.md`, preserved separate domain ledgers, and updated README, Context, Bootstrap, TODO, and Decision Log so fresh-chat restoration selects and evaluates each domain independently.

### FDW-TODO-002 — Align the ChatGPT automation with durable repository state
**Priority:** High  
**Status:** DONE

Reconciled the automation to the canonical `Deal_Watch` identity and renamed it `Deal Watch — Fishing`. The fishing-specific target prompt remains an execution mechanism; repository state is authoritative.

### FDW-TODO-000 — Initialize durable project state
**Status:** DONE

Created and reconciled the core durable records plus fishing-domain watchlist, source, rule, and listing-history files.

## Next unused task ID

`DW-TODO-013`
