# Deal_Watch — New Chat Bootstrap Prompt

Copy/paste the section below into a completely fresh ChatGPT conversation inside the `Deal_Watch` project.

---

Restore the current **Deal_Watch** project state from GitHub.

Repository: `JBrickey23/Deal_Watch`  
Default branch: `main`

GitHub is the durable source of truth. Do not rely on old conversation memory when it conflicts with current repository state.

## Restore procedure

Read, in this order:
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

Then tell me concisely:
1. the current authoritative project state;
2. the active domains;
3. what work is open;
4. the immediate continuation point;
5. the next unused durable task ID;
6. whether GitHub read/write access is currently available.

Do not make repository changes until restoration is complete unless I explicitly ask you to reconcile immediately.

## Current checkpoint

`Deal_Watch` is initialized as a durable, multi-domain deal-discovery framework.

Active domains:
- **Fishing** — premium tackle bargain discovery, including the Worker rod role.
- **Hat:Machine** — purpose-built, convertible, and sleeper machines evaluated against whether they can sew a leather sweatband into a formed felt hat.

The possible felt-hat acquisition/upcycling watch remains a separately scoped future domain and is not active.

Shared records:
- `WATCHLIST.md`
- `SOURCES.md`
- durable Context, TODO, Decision Log, and Bootstrap files.

Domain records:
- Fishing: `DEAL_RULES.md`, `LISTINGS.md`
- Hat:Machine: `HAT_MACHINE_DEAL_RULES.md`, `HAT_MACHINE_LISTINGS.md`

## Domain separation rule

Select the requested domain before searching. Apply only its rules and write only to its ledger. Do not blend Fishing and Hat:Machine findings into one run or ledger.

## Current continuation

The current continuation focus is **Hat:Machine**. Search exact-purpose machines plus convertible and sleeper industrial machines, including cylinder-arm, post-bed, off-the-arm/free-arm, upholstery, leather, canvas, shoe-repair, shop-liquidation, and used-industrial-dealer sources.

For every candidate, answer the formed-hat geometry question first and identify any actual modification path and all-in cost. Record meaningful findings and actual source coverage in `HAT_MACHINE_LISTINGS.md`.

Fishing remains active and can be run separately.

## Automation state

A daily condition-watch automation named `Deal Watch — Fishing` is enabled for Fishing. It is only an execution mechanism. No Hat:Machine automation is assumed unless separately created.

## Naming and cleanup

The canonical project name is `Deal_Watch`. Fishing and Hat:Machine are domain labels. Existing `FDW-*` IDs remain stable; new durable IDs use `DW-*`.

Old chats can be deleted only after important decisions, listings, source findings, rule changes, and continuation details have been reconciled into GitHub.

## Do not repeat

Do not recreate project initialization. Do not treat unchanged or previously rejected listings as new. Do not claim a source was searched when it was inaccessible or not searched.

---
