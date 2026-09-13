# Fishing Deal Watch — TODO

Canonical list of unfinished, blocked, waiting, or deferred work. IDs are never reused.

## OPEN

### FDW-TODO-001 — Validate source coverage across real runs
**Priority:** High  
**Status:** OPEN

Run the watch repeatedly using the source checklist in `SOURCES.md` and determine which sources are reliably searchable, intermittently searchable, login-limited, or effectively inaccessible from ChatGPT.

Success criteria:
- coverage status is known for every primary source;
- reports distinguish `SEARCHED`, `INACCESSIBLE`, and `NOT SEARCHED`;
- source rules are updated from evidence rather than assumptions.

### FDW-TODO-002 — Align the ChatGPT automation with durable repository state
**Priority:** High  
**Status:** OPEN

The existing daily `Fishing Deal Watch` automation contains a long embedded watchlist. Reconcile it so repository files are the authoritative durable specification and the automation does not silently diverge.

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

### FDW-TODO-000 — Initialize durable project state
**Status:** DONE

Created and reconciled the core durable records plus Fishing Deal Watch-specific watchlist, source, rule, and listing-history files.

## Next unused task ID

`FDW-TODO-006`
