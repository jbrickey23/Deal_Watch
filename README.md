# Deal_Watch

`Deal_Watch` is a durable GitHub-backed project for finding, verifying, evaluating, and tracking unusually good deals across multiple watch domains.

## Active domains

### Fishing
Bargain discovery for premium fishing tackle, emphasizing older, discontinued, misidentified, or materially undervalued rods and reels. The named `Worker` rod role remains a high-priority target.

- Targets: `WATCHLIST.md` → `Domain — Fishing`
- Rules: `DEAL_RULES.md`
- Ledger: `LISTINGS.md`

### Hat:Machine
Discovery of machines that can sew a leather sweatband into a formed felt hat. It covers purpose-built machines, credible conversions, and poorly identified sleeper machines.

- Targets: `WATCHLIST.md` → `Domain — Hat:Machine`
- Rules: `HAT_MACHINE_DEAL_RULES.md`
- Ledger: `HAT_MACHINE_LISTINGS.md`

The possible felt-hat acquisition/upcycling watch remains a separately scoped future domain. It is not the same as `Hat:Machine`.

## Durable operating model

ChatGPT conversations are working sessions. GitHub is the durable authoritative project state.

Canonical repository: `JBrickey23/Deal_Watch`

Shared state:
- `Deal_Watch_Context.md`
- `Deal_Watch_TODO.md`
- `Deal_Watch_Decision_Log.md`
- `Deal_Watch_New_Chat_Bootstrap_Prompt.md`
- `WATCHLIST.md`
- `SOURCES.md`

Domain records:
- Fishing: `DEAL_RULES.md`, `LISTINGS.md`
- Hat:Machine: `HAT_MACHINE_DEAL_RULES.md`, `HAT_MACHINE_LISTINGS.md`

## Naming principle

The canonical project name is `Deal_Watch`. Fishing and `Hat:Machine` are active watch domains, not project names. Existing `FDW-*` task and decision IDs remain unchanged as stable historical identifiers; new durable IDs use `DW-*`.

## Current workflow

1. Restore shared state and both domain records from GitHub.
2. Select the requested domain; do not silently run or merge domains.
3. Search actual sources from `SOURCES.md` for that domain's targets in `WATCHLIST.md`.
4. Evaluate candidates using the selected domain's rules.
5. Compare against the selected domain's ledger.
6. Report actual source coverage explicitly.
7. Reconcile meaningful changes into the appropriate shared and domain-specific files.

A daily ChatGPT condition-watch automation named `Deal Watch — Fishing` exists for Fishing. It is an execution mechanism; repository state is authoritative. No Hat:Machine automation is assumed unless separately created.
