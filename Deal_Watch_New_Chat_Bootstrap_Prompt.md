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
9. `Deal_Watch_New_Chat_Bootstrap_Prompt.md`

Then tell me concisely:
1. the current authoritative project state;
2. what work is open;
3. the immediate continuation point;
4. the next unused durable task ID;
5. whether GitHub read/write access is currently available.

Do not make repository changes until the restore is complete unless I explicitly ask you to reconcile immediately.

## Reconciled checkpoint additions

- Preserve full clickable listing URLs in `LISTINGS.md`; for Facebook Marketplace use `https://www.facebook.com/marketplace/item/<listing_id>/`.
- Facebook Marketplace was previously authenticated and searched around Redmond/98053, represented by Facebook as Ames Lake, within 500 miles. If the browser environment is unavailable, mark authenticated Marketplace coverage honestly rather than treating public indexed results as native coverage.
- A future felt-hat domain has been scoped but is not active. Fishing remains active unless the user explicitly asks to switch.
- Candidate felt-hat domain focus: thrift/garage-sale/estate-sale quality fur-felt hats for reshape/upcycle, especially rabbit felt, beaver felt, beaver blend, and 50/50 beaver/rabbit. Evaluate size, condition, price, material-confidence, X/XXX markings, and visual evidence from sweatband/liner/tags/photos.

## Current checkpoint

`Deal_Watch` is initialized as a durable GitHub-backed deal-discovery framework. Fishing is the current watch domain, focused on unusually good fishing-tackle deals, particularly older, discontinued, misidentified, or undervalued premium tackle.

The durable project includes:
- an authoritative watchlist;
- a source checklist with explicit coverage-state reporting;
- deal-scoring and verification rules;
- a listing/history ledger;
- durable tasks and decisions.

A daily ChatGPT automation named `Deal Watch — Fishing` is enabled for the current fishing domain. Treat it as an execution mechanism, not the durable source of truth.

## Naming rule

The canonical project name is `Deal_Watch`. The repository is `JBrickey23/Deal_Watch`. Fishing is a watch domain, not a project rename. Do not silently substitute `Fishing Deal Watch`, `Fishing_Deal_Watch`, `Deal_Watcher`, or another alias for the canonical project name.

Existing `FDW-*` durable IDs are legacy stable identifiers and remain unchanged. New durable IDs use `DW-*`.

## Chat cleanup rule

Old chat windows are working sessions, not durable records. They can be deleted after any important decisions, actions, listings, source findings, rule changes, or continuation details from that chat have been reconciled into the GitHub repository.

When in doubt, reconcile first and delete the old chat only after confirming the repository either changed appropriately or already contained the relevant state.

## Do not repeat

Do not recreate project initialization. Do not treat previously rejected fair-market listings as new finds unless price, condition, identity, or availability has materially changed.

Do not claim a source was searched when it was inaccessible or not searched.

## Current operating priorities

- Use `WATCHLIST.md` for fishing-domain targets.
- Use `SOURCES.md` for search coverage and discovery/verification roles.
- Use `DEAL_RULES.md` for delivered-price discipline, verification, risk analysis, and Deal Scores.
- Use `LISTINGS.md` to detect new, changed, ended, or already-rejected listings.

## Immediate continuation

The next substantive fishing-domain search run should execute against the durable repository specification, report actual source coverage, and update `LISTINGS.md` with worthwhile new or meaningfully changed observations.

After meaningful work, reconcile affected durable records before transferring to another conversation.

---
