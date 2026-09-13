# Deal_Watch

`Deal_Watch` is a durable GitHub-backed project for finding, verifying, evaluating, and tracking unusually good deals from curated watchlists and source sets.

Fishing is the current watch domain. It emphasizes `garage-find` opportunities: older, discontinued, misidentified, or materially undervalued premium tackle. Fair-market listings are useful as benchmarks but are not the primary goal.

## Durable operating model

ChatGPT conversations are working sessions. GitHub holds the durable authoritative project state.

Canonical repository: `JBrickey23/Deal_Watch`

Core state:
- `Deal_Watch_Context.md`
- `Deal_Watch_TODO.md`
- `Deal_Watch_Decision_Log.md`
- `Deal_Watch_New_Chat_Bootstrap_Prompt.md`

Project-specific records:
- `WATCHLIST.md` — authoritative targets and reference configurations for the active watch domain
- `SOURCES.md` — source checklist, roles, and coverage-reporting rules
- `DEAL_RULES.md` — scoring, verification, price, and notification rules
- `LISTINGS.md` — durable listing/history ledger and market benchmarks

## Naming principle

The canonical project name is `Deal_Watch`. Domain labels such as `Fishing` describe what is currently being watched and must not silently become new project names. Existing `FDW-*` task and decision IDs remain unchanged as stable historical identifiers; new durable IDs use `DW-*`.

## Current workflow

1. Restore current state from GitHub.
2. Search actual sources from `SOURCES.md` for targets in `WATCHLIST.md`.
3. Evaluate promising listings using `DEAL_RULES.md`.
4. Compare against `LISTINGS.md` to identify what is genuinely new or changed.
5. Report actual source coverage explicitly.
6. Reconcile durable records after meaningful changes.

A daily ChatGPT condition-watch automation named `Deal Watch — Fishing` exists for the current fishing domain. It is an execution mechanism; repository state is authoritative.

For a completely fresh conversation, use `Deal_Watch_New_Chat_Bootstrap_Prompt.md`.
