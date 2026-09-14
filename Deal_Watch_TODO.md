# Deal_Watch — TODO

Canonical list of unfinished, blocked, waiting, or deferred work. IDs are never reused.

Legacy `FDW-*` IDs are preserved as stable historical identifiers. New task IDs use the `DW-*` prefix.

## OPEN

### DW-TODO-006 — Verify ChatGPT Project Instructions after canonical rename
**Priority:** High  
**Status:** OPEN

Verify that the ChatGPT Project named `Deal_Watch` uses the canonical repository `JBrickey23/Deal_Watch` and the renamed durable files (`Deal_Watch_Context.md`, `Deal_Watch_TODO.md`, `Deal_Watch_Decision_Log.md`, and `Deal_Watch_New_Chat_Bootstrap_Prompt.md`). Remove any stale `Fishing_Deal_Watch`, `Fishing Deal Watch`, or `Deal_Watcher` references that incorrectly identify the project rather than the fishing watch domain.

Success criteria:
- ChatGPT Project name is `Deal_Watch`;
- Project Instructions reference `JBrickey23/Deal_Watch`;
- restore/reconcile instructions use the canonical `Deal_Watch_*` filenames;
- Fishing is represented as a watch domain, not the project identity.

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

### FDW-TODO-002 — Align the ChatGPT automation with durable repository state
**Priority:** High  
**Status:** DONE

Reconciled the automation to the canonical `Deal_Watch` identity and renamed it `Deal Watch — Fishing`. The fishing-specific target prompt remains an execution mechanism; repository state is authoritative.

### FDW-TODO-000 — Initialize durable project state
**Status:** DONE

Created and reconciled the core durable records plus fishing-domain watchlist, source, rule, and listing-history files.

## Next unused task ID

`DW-TODO-007`
