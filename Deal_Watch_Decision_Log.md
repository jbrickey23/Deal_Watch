# Deal_Watch — Decision Log

Newest decisions first. Record durable decisions, not every discussion.

Legacy `FDW-*` IDs remain stable historical identifiers. New decision IDs use the `DW-*` prefix.

## DW-DEC-014 — Define the Worker go-to light spinning role
**Date:** 2026-09-15  
**Status:** Current

Add `Worker` as a named fishing-domain rod role/specification class rather than a single model. The Worker is intended to be the go-to light spinning rod when the exact target species or presentation is not known: panfish and trout through finesse/general light-duty bass, while existing heavier rods cover bigger lures, heavy cover, and larger-fish work.

Worker preferences are maintained authoritatively in `WATCHLIST.md`. Key durable characteristics are Medium-Light power, Fast/Extra Fast action, approximately 6'8"–7'2", strong preference for 2-piece transportability, good performance around 1/8 oz with useful upper range through at least 3/8 and preferably 1/2–5/8 oz, shorter rear handle, and continuous/full cork when available.

For the Worker role specifically, 2-piece construction carries more ranking weight than it does in the general rod framework. Exceptional 1-piece rods can still be surfaced but must be identified as a transport compromise.

Current Fenwick Worker anchors:
- `EGLW70ML-FS-2` at about $99.95 new is the value baseline.
- `HMGW72ML-FS-2` at about $179.95 new is the current performance benchmark.

Deal_Watch should search beyond these exact SKUs, including current and prior Eagle/HMG/Elite/Walleye/Inshore/general Fenwick spinning rods and poorly identified used listings whose photos/specifications fit the Worker role.

## DW-DEC-013 — BidRush is a promising validated source
**Date:** 2026-09-15  
**Status:** Current

BidRush should be included as a Deal_Watch discovery source. A direct test of `https://bidrush.com/items/vintage-men-s-hats-KYK5H9` returned `200 OK` and exposed machine-readable listing details in the page HTML, including title, description, location, listing status, end time, highest bid, bid count, pickup/shipping flags, auction metadata, and image URLs.

Treat BidRush as promising for local/estate-style auction discovery across watch domains, including the current fishing domain and possible future thrift/upcycle felt-hat domain. Direct item-page reading is validated from this example; broader BidRush search coverage should still be validated during future runs and reported honestly in source coverage.

## DW-DEC-011 — Preserve full clickable listing URLs and evidence links
**Date:** 2026-09-14  
**Status:** Current

Notable listing entries must preserve a full clickable URL whenever available, not only source names, search terms, listing titles, or relative hrefs.

For Facebook Marketplace, store stable item links as:

`https://www.facebook.com/marketplace/item/<listing_id>/`

Also preserve the listing ID, observed title, price, location, source/search scope, and verification status. Search-result tracking query strings are not needed for durable item links unless they are the only way to recover the listing.

Authenticated Marketplace coverage must be reported truthfully. Public indexed Facebook results are not equivalent to native authenticated Marketplace searching.

## DW-DEC-012 — Felt hats are a candidate future domain, not the active domain
**Date:** 2026-09-14  
**Status:** Current

A possible future watch domain for thrift/garage-sale quality felt hats was scoped but not activated. Fishing remains the current active domain until the user explicitly requests a domain switch.

The felt-hat domain should target reshape/upcycle candidates, especially rabbit felt, beaver felt, beaver blends, and explicit 50/50 beaver/rabbit felt. Early value guidance: verified quality fur felt under $100 is generally interesting, with thresholds to be refined from observed listings.

Hat verification should prioritize visible material markings, size, condition, price, and upcycle potential. X/XXX ratings are useful clues but not standardized across brands or eras; exact material markings carry more confidence than X-count alone.

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
