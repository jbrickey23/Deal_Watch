# Fishing Deal Watch — New Chat Bootstrap Prompt

Copy/paste the section below into a completely fresh ChatGPT conversation inside the Fishing Deal Watch project.

---

Restore the current **Fishing_Deal_Watch** project state from GitHub.

Repository: `JBrickey23/Fishing_Deal_Watch`  
Default branch: `main`

GitHub is the durable source of truth. Do not rely on old conversation memory when it conflicts with current repository state.

## Restore procedure

Read, in this order:
1. `README.md`
2. `Fishing_Deal_Watch_Context.md`
3. `Fishing_Deal_Watch_TODO.md`
4. `Fishing_Deal_Watch_Decision_Log.md`
5. `WATCHLIST.md`
6. `SOURCES.md`
7. `DEAL_RULES.md`
8. `LISTINGS.md`
9. `Fishing_Deal_Watch_New_Chat_Bootstrap_Prompt.md`

Then tell me concisely:
1. the current authoritative project state;
2. what work is open;
3. the immediate continuation point;
4. the next unused durable task ID;
5. whether GitHub read/write access is currently available.

Do not make repository changes until the restore is complete unless I explicitly ask you to reconcile immediately.

## Current checkpoint

Fishing Deal Watch is initialized as a durable GitHub-backed project for finding and evaluating unusually good fishing-tackle deals. It prioritizes older, discontinued, misidentified, or undervalued premium tackle rather than generic shopping results.

The durable project includes:
- an authoritative watchlist;
- a source checklist with explicit coverage-state reporting;
- deal-scoring and verification rules;
- a listing/history ledger;
- durable tasks and decisions.

A daily ChatGPT automation named `Fishing Deal Watch` already exists and is enabled. Treat it as an execution mechanism, not the durable source of truth. Its embedded prompt may lag the repository until `FDW-TODO-002` is resolved.

## Do not repeat

Do not recreate project initialization. Do not treat previously rejected fair-market listings as new finds unless price, condition, identity, or availability has materially changed.

Do not claim a source was searched when it was inaccessible or not searched.

## Current operating priorities

- Use `WATCHLIST.md` for targets.
- Use `SOURCES.md` for search coverage and discovery/verification roles.
- Use `DEAL_RULES.md` for delivered-price discipline, verification, risk analysis, and Deal Scores.
- Use `LISTINGS.md` to detect new, changed, ended, or already-rejected listings.

## Immediate continuation

The next substantive search run should execute against the durable repository specification, report actual source coverage, and update `LISTINGS.md` with worthwhile new or meaningfully changed observations.

After meaningful work, reconcile affected durable records before transferring to another conversation.

---
