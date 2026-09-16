# Deal_Watch

`Deal_Watch` is a durable GitHub-backed project for finding, verifying, evaluating, and tracking unusually good deals through explicitly named watch keys.

## Canonical naming

Canonical watch identifiers use:

`Project:Domain:WatchType`

Inside this repository, the project-qualified prefix may be omitted when context is unambiguous:

`Domain:WatchType`

Current canonical watch keys:
- `Deal_Watch:Fishing:WorkerRod`
- `Deal_Watch:Fishing:StradicReel`
- `Deal_Watch:Hat:SweatbandMachine`

Broad labels such as `Fishing`, `Hat`, `Worker`, or `Machine` are organizational terms or historical shorthand, not complete watch identifiers.

## Active watches

### Fishing:WorkerRod
The go-to light spinning-rod watch: Medium-Light preferred, Fast/Extra Fast, approximately 6'8"–7'2", strongly preferred 2-piece construction, shorter rear handle, and full cork when available. Named Shimano, Fenwick, and G. Loomis targets are evaluated against this role rather than treated as an unrelated generic fishing watch.

### Fishing:StradicReel
Shimano Stradic FM 1000- and 2500-size reel targets, with exact SKU, delivered-price, condition, and transaction-risk verification.

### Hat:SweatbandMachine
Purpose-built, convertible, and sleeper machinery evaluated against whether it can sew a leather sweatband into a formed felt hat.

The separately discussed felt-hat acquisition/upcycling watch is inactive. If activated, its intuitive key is `Hat:FeltHat`.

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

Stable storage files:
- Fishing watch rules/history: `DEAL_RULES.md`, `LISTINGS.md`
- `Hat:SweatbandMachine` rules/history: `HAT_MACHINE_DEAL_RULES.md`, `HAT_MACHINE_LISTINGS.md`

The existing filenames remain stable storage names. Canonical watch identity comes from the qualified keys, not from filenames.

## Current workflow

1. Restore current GitHub state.
2. Identify the requested canonical watch key.
3. Search the applicable sources and targets.
4. Apply only that watch's rules and comparisons.
5. Write findings to the correct ledger and label entries with the watch key.
6. Report actual source coverage.
7. Reconcile meaningful changes.

A legacy daily automation named `Deal Watch — Fishing` currently executes the Fishing watches. Its broad name should not be used as the naming model for new watches; automation naming/splitting remains a separate operational cleanup item.
