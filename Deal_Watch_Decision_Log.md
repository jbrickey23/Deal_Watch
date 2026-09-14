# Deal_Watch — Decision Log

Newest decisions first. Record durable decisions, not every discussion.

Legacy `FDW-*` IDs remain stable historical identifiers. New decision IDs use the `DW-*` prefix.

## DW-DEC-010 — Old chats are disposable only after reconciliation
**Date:** 2026-09-14  
**Status:** Current

ChatGPT conversations are working sessions, not durable project records. Durable state lives in the GitHub repository files.

Before deleting an old chat, assume any unreconciled decisions, actions, listings, source findings, rule changes, or continuation details that exist only in that chat may be lost from the project record. When unsure, reconcile the chat into `Deal_Watch` first, then delete it after confirming the repository either changed appropriately or already contained the relevant state.

A specific phrase such as `reconcile Deal_Watch` is a reliable trigger, but the important requirement is the action: review the session and update the affected durable repository records.

## DW-DEC-009 — Watch properties use REQUIRED, PREFERRED, and EXCLUDE levels
**Date:** 2026-09-13  
**Status:** Current

Watchlist properties may be assigned one of three behavioral levels:
- `REQUIRED` — must be satisfied for specification-driven discovery unless a named priority target explicitly documents an exception;
- `PREFERRED` — improves relevance/ranking but is not mandatory;
- `EXCLUDE` — hard rejection when the property is verified.

If a material REQUIRED or EXCLUDE property cannot be established from the listing, record it as `UNVERIFIED` rather than assuming eligibility. A potentially strong listing may be surfaced specifically because verification is needed.

This structure lets the watch evolve from broad discovery into precise filtering without forcing every useful preference to become a hard rule.

## DW-DEC-008 — Rod discovery uses specifications plus named priority targets
**Date:** 2026-09-13  
**Status:** Current

Rod discovery must not be limited to an exhaustive list of known model names. Organize the fishing-domain rod watch as a layered search:
- preferred brands;
- broad preferred specifications and qualities;
- named high-priority model families/exact models;
- opportunistic comparable finds.

Current rod properties are maintained authoritatively in `WATCHLIST.md` using the REQUIRED/PREFERRED/EXCLUDE semantics established by `DW-DEC-009`.

Preferred brands currently include Shimano, Fenwick, and G. Loomis. Named models remain priority targets and useful value anchors, but unfamiliar rods that credibly match the watch-property profile and present unusually strong value should also be surfaced.

## DW-DEC-007 — Canonical naming consistency
**Date:** 2026-09-13  
**Status:** Current

The canonical project name is `Deal_Watch`, with repository `JBrickey23/Deal_Watch`. Fishing is the current watch domain, not the project name. Descriptive aliases such as `Fishing Deal Watch`, `Fishing_Deal_Watch`, or `Deal_Watcher` must not silently become canonical names.

Existing `FDW-*` task and decision IDs are preserved because durable IDs should remain stable. New durable IDs use the `DW-*` prefix.

## FDW-DEC-006 — Defer software automation until search workflow is proven
**Date:** 2026-09-13  
**Status:** Current

Do not build collectors, GitHub Actions, or a custom application yet. First operate the durable workflow across repeated runs and identify actual limitations. Revisit after roughly 10–20 runs.

## FDW-DEC-005 — Preserve source-coverage truth explicitly
**Date:** 2026-09-13  
**Status:** Current

Every substantive search run should distinguish sources actually searched from sources inaccessible or not searched. `Nothing found` must never be used to imply a source was checked when it was not.

Preferred states:
- `SEARCHED`
- `INACCESSIBLE`
- `NOT SEARCHED`

## FDW-DEC-004 — Preserve listing lifecycle/history
**Date:** 2026-09-13  
**Status:** Current

Known listings should retain history rather than being rediscovered from scratch. Useful lifecycle states include:
- `NEW`
- `PRICE DROP`
- `STILL AVAILABLE`
- `SOLD/ENDED`
- `REJECTED`

## FDW-DEC-003 — Delivered price and verifiability drive deal scoring
**Date:** 2026-09-13  
**Status:** Current

Deal Score is based on acquisition value, not product quality alone. Delivered price, exact-model confidence, condition, transaction/seller risk, and realistic market value all matter. Shipping is part of acquisition cost.

A mislabeled listing can become more interesting when photos credibly indicate a better product than the seller recognizes.

## FDW-DEC-002 — GitHub is the durable source of truth
**Date:** 2026-09-13  
**Status:** Current

Use the Durable_CHATGPT operating pattern for `Deal_Watch`. ChatGPT conversations are working sessions; GitHub stores authoritative watch targets, rules, source coverage, listing history, open tasks, and handoff state.

Scheduled ChatGPT automations are execution mechanisms, not the durable authority.

## FDW-DEC-001 — Define the fishing watch as bargain discovery, not generic shopping
**Date:** 2026-09-13  
**Status:** Current

The fishing domain should prioritize `garage-find` style opportunities: undervalued, older, discontinued, misidentified, or unusually discounted fishing tackle. Fair market pricing is useful as a benchmark but normally should not trigger a deal alert.
