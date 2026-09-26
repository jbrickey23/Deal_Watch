# Deal_Watch — New Chat Bootstrap Prompt

Copy/paste the section below into a completely fresh ChatGPT conversation inside the `Deal_Watch` project.

---

Restore the current **Deal_Watch** project state from GitHub.

Repository: `JBrickey23/Deal_Watch`  
Default branch: `main`

GitHub is the durable source of truth. Do not rely on old conversation memory when it conflicts with current repository state.

GitHub write note: normal UTF-8 file edits can use `fetch_file` plus `update_file` / `create_file`. Binary assets require the Git object path: `create_blob` with base64 content, `create_tree`, `create_commit`, then `update_ref` to fast-forward `main`. This was verified in commit `33c24c8e1a9624ce891512b471a63cc32ee73437`.

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
11. `REEL_IMAGES.md`
12. `FISHING_INVENTORY.md`
13. `Deal_Watch_New_Chat_Bootstrap_Prompt.md`

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

Active canonical watches:
- `Deal_Watch:Fishing:WorkerRod`
- `Deal_Watch:Fishing:StradicReel`
- `Deal_Watch:Hat:SweatbandMachine`

The possible felt-hat acquisition/upcycling watch remains a separately scoped future domain and is not active.

Shared records:
- `WATCHLIST.md`
- `SOURCES.md`
- durable Context, TODO, Decision Log, and Bootstrap files.

Domain records:
- Fishing: `DEAL_RULES.md`, `LISTINGS.md`
- Hat:SweatbandMachine: `HAT_MACHINE_DEAL_RULES.md`, `HAT_MACHINE_LISTINGS.md`

## Watch-key separation rule

Select the requested canonical watch key before searching. Apply only its rules and label findings with that key. Do not blend Fishing and Hat:SweatbandMachine findings into one run or ledger.

## Current continuation

The latest continuation focus is **owned Fishing inventory and the `EGLW66M-FS-2` keep/return decision**. Read `FISHING_INVENTORY.md` and the 2026-09-26 session handoff in `Deal_Watch_Context.md` first for the current corrections and open questions. `Deal_Watch:Hat:SweatbandMachine` remains active for a separately requested run. Search exact-purpose machines plus convertible and sleeper industrial machines, including cylinder-arm, post-bed, off-the-arm/free-arm, upholstery, leather, canvas, shoe-repair, shop-liquidation, and used-industrial-dealer sources.

For every candidate, answer the formed-hat geometry question first and identify any actual modification path and all-in cost. Record meaningful findings and actual source coverage in `HAT_MACHINE_LISTINGS.md`.

`Deal_Watch:Fishing:WorkerRod` and `Deal_Watch:Fishing:StradicReel` remain active and can be run separately.

## Automation state

A daily condition-watch automation named `Deal Watch — Fishing` is enabled for Fishing. It is only an execution mechanism. No Hat:SweatbandMachine automation is assumed unless separately created.

## Naming and cleanup

The canonical project name is `Deal_Watch`. `Fishing` and `Hat` are domains; `WorkerRod`, `StradicReel`, and `SweatbandMachine` are watch types. Domain-only labels are not canonical watch identifiers. Existing `FDW-*` IDs remain stable; new durable IDs use `DW-*`.

Old chats can be deleted only after important decisions, listings, source findings, rule changes, and continuation details have been reconciled into GitHub.

## Do not repeat

Do not recreate project initialization. Do not treat unchanged or previously rejected listings as new. Do not claim a source was searched when it was inaccessible or not searched.

---
