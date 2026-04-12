# Google Ads Fundamentals

## Contents

- [Search vs Interruption Advertising](#search-vs-interruption-advertising)
- [How Google's Auction Works](#how-googles-auction-works)
- [Quality Score](#quality-score)
- [Smart Bidding](#smart-bidding)
- [Conversion Tracking](#conversion-tracking)
- [The Feedback Loop](#the-feedback-loop)

---

## Search vs Interruption Advertising

Google Search is **intent-based**: ads appear when someone actively searches for what you sell. This makes it fundamentally different from Meta or TikTok.

|                     | Search (Google)                              | Interruption (Meta, TikTok)                      |
| ------------------- | -------------------------------------------- | ------------------------------------------------ |
| **When ads show**   | When the user types a relevant query         | Between content the user chose to consume        |
| **Audience intent** | High — actively seeking a solution           | Low — wasn't looking for you                     |
| **Conversion rate** | Higher (warm/hot traffic)                    | Lower (cold traffic)                             |
| **Reach ceiling**   | Capped by search volume for your keywords    | Massive — limited only by platform users         |
| **Core challenge**  | Relevance: keyword → ad → landing page       | Creative: stop the scroll                        |

**Use Google Search when:** buyers are actively searching for your category. "Project management software", "Salesforce alternative", "time tracking tool for agencies" — all high-intent searches.

**Use both when:** budget allows. Google captures existing demand; interruption platforms create new demand.

---

## How Google's Auction Works

Google's auction is not purely a price war. The ranking formula is:

```
Ad Rank = Bid × Quality Score × Expected Impact of Extensions
```

A higher Quality Score lets you win auctions at a **lower CPC** than competitors who bid more. This is the core opportunity: you can outcompete bigger spenders by being more relevant.

**Implications:**
- Wasting budget on irrelevant clicks destroys Quality Score
- A tight keyword → ad → landing page system beats a "bid more" strategy
- Ad Strength (Google's diagnostic metric) is not Quality Score — don't optimize for it

---

## Quality Score

Quality Score is Google's 1–10 rating of your ad's relevance, measured per keyword. It affects both your CPC and your position.

Three components:

| Component                   | What Google measures                                      |
| --------------------------- | --------------------------------------------------------- |
| **Expected CTR**            | Will searchers click this ad for this keyword?            |
| **Ad Relevance**            | Does the ad match the intent behind the keyword?          |
| **Landing Page Experience** | Does the landing page deliver on the ad's promise?        |

**How to improve it:** keep keyword, ad copy, and landing page tightly aligned. One ad group per theme → one landing page per ad group. The tighter the relevance chain, the higher the score.

**What Quality Score is not:** a content writing exercise. Keyword-stuffing headlines doesn't help. Genuine relevance does.

---

## Smart Bidding

Smart bidding (Target CPA, Target ROAS, Maximize Conversions) uses Google's ML to optimize bids in real time. It works — but only with enough conversion data.

**Minimum thresholds before switching to smart bidding:**
- Target CPA: 30–50 conversions/month per campaign
- Target ROAS: 50+ conversions/month with revenue data

Below these thresholds, use **Maximize Clicks** (with a bid cap) or **Manual CPC** to gather data before handing control to the algorithm.

**Never launch a new account on Target CPA.** The algorithm has no baseline — it will either underspend (too cautious) or overspend (no guardrails). Start manual, earn data, then graduate.

---

## Conversion Tracking

Smart bidding is only as good as the signal feeding it. Accurate conversion tracking is non-negotiable.

**What to track:**
- Primary conversions: trial signups, demo requests, purchases (used for bidding)
- Secondary conversions: form fills, PDF downloads (observational only — don't use for bidding)

**Enhanced Conversions:** send hashed customer data (email) back to Google alongside conversion events. Improves match rate significantly, especially with iOS/cookie restrictions. Enable before launching.

**Warning:** if you import Google Analytics goals as conversions, verify they're not double-counting. GA sessions-based goals and Google Ads conversion windows can overlap.

---

## The Feedback Loop

Google Search runs on a tight feedback loop: **Launch → Analyze → Refine.**

- Every week, the Search Term Report shows you what people actually typed
- You decide: promote to keyword / add as negative / ignore
- Better negatives → less wasted spend → higher Quality Score → lower CPC
- Better keywords → more relevant ad groups → better landing page alignment

The loop doesn't stop. Drift is constant — query distributions shift as competitors enter, seasons change, and your product evolves. Weekly review for 60 days, monthly after that.
