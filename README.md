# Fishing_Deal_Watch

Fishing Deal Watch is a durable GitHub-backed project for finding, verifying, and evaluating unusually good fishing-gear deals from a curated watchlist and source set.

The project emphasizes `garage-find` opportunities: older, discontinued, misidentified, or materially undervalued premium tackle. Fair-market listings are useful as benchmarks but are not the primary goal.

## Durable operating model

ChatGPT conversations are working sessions. GitHub holds the durable authoritative project state.

Core state:
- `Fishing_Deal_Watch_Context.md`
- `Fishing_Deal_Watch_TODO.md`
- `Fishing_Deal_Watch_Decision_Log.md`
- `Fishing_Deal_Watch_New_Chat_Bootstrap_Prompt.md`

Project-specific records:
- `WATCHLIST.md` — authoritative gear targets and reference configurations
- `SOURCES.md` — source checklist, roles, and coverage-reporting rules
- `DEAL_RULES.md` — scoring, verification, price, and notification rules
- `LISTINGS.md` — durable listing/history ledger and market benchmarks

## Current workflow

1. Restore current state from GitHub.
2. Search actual sources from `SOURCES.md` for targets in `WATCHLIST.md`.
3. Evaluate promising listings using `DEAL_RULES.md`.
4. Compare against `LISTINGS.md` to identify what is genuinely new or changed.
5. Report actual source coverage explicitly.
6. Reconcile durable records after meaningful changes.

A daily ChatGPT condition-watch automation named `Fishing Deal Watch` already exists. It is an execution mechanism; repository state is authoritative.

For a completely fresh conversation, use `Fishing_Deal_Watch_New_Chat_Bootstrap_Prompt.md`.
