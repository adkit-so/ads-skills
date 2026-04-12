# Analyze & Scale

The audit workflow for a running account. The loop that keeps the relevance system tight as query distributions drift.

**Weekly for 60 days, then monthly.** No exceptions.

---

## Search Term Report (STR) Audit

Pull configuration:

- **Date range:** last 30 days (or matching your reporting cadence)
- **Status filter:** None — only terms not yet added as keyword or negative. Don't re-evaluate past decisions.
- **Minimum clicks:** 1 — skip zero-click noise
- **Sort:** cost descending — 80% of the waste lives in the top 20% of spend
- **Limit:** ~2,000 rows

### The Three-Way Decision

For every term, cross-reference: **the search term** (what the user typed) + **the matched keyword** (what triggered it) + **the campaign + ad group** (what theme it was supposed to serve). Ask: _does this fit the theme?_

| Decision                  | When                                                                               | What to do                                           |
| ------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------- |
| **Promote** (add keyword) | On-theme and converting (or high CTR) — reveals intent you hadn't covered          | Classify by intent (see `2-keyword-mining.md`), add to the right ad group |
| **Demote** (add negative) | Off-theme, wrong intent, brand leakage, or too generic for the ad group it landed in | Classify into the right negative list (see `5-negative-keywords.md`) |
| **Ignore**                | One-off noise, single click, no pattern                                            | No action. It'll fall off the pull next cycle.       |

**Relevance matters more than conversion count alone.** An on-theme term with zero conversions can stay. A converting term in the wrong ad group is still a negative _there_ — even if it belongs in a different ad group somewhere else.

Work top-down by cost, not row count. A term with 200 clicks at $0.10 CPC matters less than 20 clicks at $5 CPC. Stop when remaining rows don't move the account.

---

## Asset Report Audit

Run alongside the STR audit, weekly.

1. Open the Asset Report for each active RSA
2. Mark headlines rated "Low" — replace or remove
3. Add 1–2 new variants to the pool per ad group per review cycle
4. After 4–6 weeks of stable CTR/CVR — unpin progressively to let Google find new combinations

---

## Landing Page CVR Check

- Pull conversion rate by ad group
- Compare each ad group against the account median
- Ad groups below median with enough traffic (50+ clicks) need a **dedicated landing page**, not a shared one
- A generic page is almost always the root cause of below-median CVR in a tight keyword group

---

## Quality Score Audit (Monthly)

1. Add Quality Score columns (Overall, Expected CTR, Ad Relevance, Landing Page Experience) at the keyword level
2. Flag keywords scoring ≤ 5
3. Diagnose the weakest component:
   - Low Expected CTR → headline pool needs keyword echo in H1
   - Low Ad Relevance → keyword is in the wrong ad group, or ad copy doesn't mirror query
   - Low Landing Page Experience → page content doesn't match what the ad promises

---

## Scaling Signals

Do **all three** before increasing budget:

- [ ] CPA at or below target for 2+ consecutive weeks
- [ ] Conversion volume ≥ 30/month per campaign (minimum for smart bidding to work)
- [ ] Search Impression Share < 60% (room left to grow before hitting the ceiling)

If Search IS > 60% and CPA is healthy, the growth lever is **new ad groups** (new themes, new intent pockets) — not higher bids.

### How to Scale

- Increase budget **20–30% at a time**. Wait 7 days before the next increase.
- **Never change bids and budget simultaneously** — you can't diagnose what moved CPA.
- **New ad groups beat higher bids** for sustainable scale. More themes = more impression surface.

### Auction Insights (Review Monthly)

Check for:
- New competitors entering your terms
- Impression share shifts (you losing ground or gaining it)
- Outranking share drops — may indicate a quality score problem, not a bid problem
