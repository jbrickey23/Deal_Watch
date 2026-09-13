# Fishing Deal Watch — Decision Log

Newest decisions first. Record durable decisions, not every discussion.

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

Use the Durable_CHATGPT operating pattern for Fishing Deal Watch. ChatGPT conversations are working sessions; GitHub stores authoritative watch targets, rules, source coverage, listing history, open tasks, and handoff state.

The scheduled ChatGPT automation is an execution mechanism, not the durable authority.

## FDW-DEC-001 — Define Fishing Deal Watch as bargain discovery, not generic shopping
**Date:** 2026-09-13  
**Status:** Current

The project should prioritize `garage-find` style opportunities: undervalued, older, discontinued, misidentified, or unusually discounted fishing tackle. Fair market pricing is useful as a benchmark but normally should not trigger a deal alert.
