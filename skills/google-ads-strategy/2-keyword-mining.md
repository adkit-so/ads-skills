# Keyword Mining

Mining produces a keyword list grouped by theme and filtered by intent. Two entry points share one pipeline: **external** sources work at launch when the account has no data; **internal** sources join once the account is running. Classify → filter → group is identical for both.

## Sources

Ranked by authority. Real queries come from real people — Keyword Planner recycles vocabulary Google already knows, not what your customers actually say.

### External (use at launch)

- **Customer interviews and sales calls** — verbatim language customers use to describe their problems. Strongest source: if 5+ customers use the same phrase unprompted, bid on it.
- **Review sites** (G2, Capterra, Product Hunt, App Store) — mine review titles first, then body text. Use your own reviews and competitor reviews.
- **Competitor landing pages and ads** — terms competitors defend in paid or organic are worth investigating. Run a keyword gap analysis against 3–5 competitors.
- **Google Autosuggest + People Also Ask** — real queries Google has observed. Type 1–3 word seeds and harvest completions.

### Internal (join once the account is live)

- **Google Search Console** — queries with ≥10 impressions and ≥1 click over the last 90 days. Pre-validated intent, no speculation.
- **Search Term Report** — terms in your account that aren't yet added as a keyword or negative. Filter to converters and high-CTR rows.
- **Site search logs** — what visitors type once they're already on your site. Often surfaces vocabulary nobody else has.

### Keyword Planner

Volume estimates and CPC ranges only. Never use it as the primary discovery source — it recycles popular vocabulary, not buyer language.

---

## Classify by Intent

Every candidate belongs to one of four buckets. Paid budget concentrates on **transactional + commercial**. Informational belongs to SEO. Navigational belongs to a dedicated brand campaign.

| Intent           | Pattern                                                                   | Paid priority           |
| ---------------- | ------------------------------------------------------------------------- | ----------------------- |
| **Transactional**| `[category] software`, `buy [x]`, `[competitor] pricing`, `free trial [x]`| Primary                 |
| **Commercial**   | `best [x]`, `[competitor] alternative`, `[x] vs [y]`, `[JTBD phrase] tool`| Primary                 |
| **Informational**| `what is [x]`, `how to [task]`, `[topic] guide`                           | Send to SEO, not paid   |
| **Navigational** | Brand + variants                                                           | Separate brand campaign |

A candidate straddling two buckets belongs to the higher-intent one.

---

## Screening

Three tests every candidate must pass. Be ruthless — a cheap bad keyword is still bad.

1. **Intent to buy in 2 months** — does someone typing this have intent to buy software like yours within ~2 months? If no, cut.
2. **Long-tail preference** — prefer 3+ word candidates over bare category nouns. They target better and cost less per click.
3. **Retargeting potential** — if the person might convert later on a different channel, the data from the click is still worth something.

---

## Group into Ad Groups

One JTBD (job-to-be-done) per ad group. Each ad group maps to one ad copy and one landing page. Usually ≤15 keywords per group — more than that means you likely have two themes and should split.

See `3-account-structure.md` for the campaign and ad group logic.

---

## Quick Reference

- **External sources:** interviews · reviews · competitor LPs · autosuggest — available at launch
- **Internal sources:** Search Console · STR · site search — once data exists
- **Keyword Planner:** sizing only, never discovery
- **Intent → paid:** transactional / commercial first · informational = SEO · navigational = brand campaign
- **Screening:** 2-month intent-to-buy · long-tail · retargeting potential
- **Grouping:** one JTBD per ad group, ≤15 keywords
