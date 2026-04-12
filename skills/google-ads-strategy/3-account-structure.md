# Account Structure

## Campaign & Ad Group Logic

**Campaigns by intent/control. Ad groups by feature/theme.**

Create campaigns based on control boundaries, not features:

- Split campaigns only when they need different **budget, bidding, geo, language, or reporting**
- Group by **traffic type / intent bucket** (brand, competitor, solution-aware, problem-aware)
- Ad groups map to **feature / theme / landing page**

**Ad group sizing:** one ad has to speak to every keyword in the group, so keep themes tight. If you're past ~15 keywords, you probably have two themes — split. Under ~5 keywords often means not enough impressions to learn anything meaningful.

**Never mix intents in one ad group** — bidding logic and landing page strategy diverge too much. Keep intents split at the campaign level so every ad group sits inside one intent by construction.

---

## Campaign Types — B2B SaaS

| Campaign       | What it targets                    | Notes                                                                                     |
| -------------- | ---------------------------------- | ----------------------------------------------------------------------------------------- |
| **Brand**      | Your brand name + variants         | Bid even if you rank organically — competitors will otherwise serve above your result. Cheapest click in the account. |
| **Competitor** | Named competitor terms             | Requires comparison landing pages. Separate budget and bidding from solution campaigns.   |
| **Solution**   | Solution-aware, high intent        | Core budget. Transactional + commercial keywords. Largest allocation.                     |
| **Problem**    | Problem-aware, longer funnel       | Lower intent, lower bids. Feeds the pipeline but converts slower.                        |

---

## Budget Split — New Account (Days 0–60)

Reference example at €5K/month:

| Campaign       | Budget       | Why                                                    |
| -------------- | ------------ | ------------------------------------------------------ |
| **Brand**      | 10% · €500   | Defensive — protect your brand terms                   |
| **Competitor** | 20% · €1,000 | High-intent alternative/vs traffic                     |
| **Solution**   | 50% · €2,500 | Primary volume driver                                  |
| **Problem**    | 20% · €1,000 | Longer funnel, lower CPA expectations                  |

**After 60 days:** rebalance on the signal closest to revenue — trial→paid for self-serve SaaS, closed-won for sales-led B2B. Don't rebalance on raw clicks or signup count — that rewards cheap traffic, not quality.

---

## Match Type Decision Table

| Scenario                                                  | Match type                                  | Why                                                                                      |
| --------------------------------------------------------- | ------------------------------------------- | ---------------------------------------------------------------------------------------- |
| Budget under $10K/month                                   | Exact + Phrase only                         | Not enough data for broad match to learn. Every wasted dollar hurts.                    |
| Under 30 conversions/month                                | Exact + Phrase only                         | Broad match needs 30+ conversions/month minimum to optimize.                            |
| $10K–$25K budget, 30+ conversions                         | Phrase + selective Broad on top keywords    | Test broad on highest-volume keywords only. Monitor weekly.                              |
| $25K+ budget, 50+ conversions, Enhanced Conversions live  | Broad match on proven keyword themes        | Algorithm has enough signal to find new converting queries autonomously.                  |
| Scaling $50K+                                             | Broad as primary, Exact as control          | At scale, broad finds queries you'd never discover with exact. Exact serves as benchmark.|

---

## Ad Group Naming Convention

Name ad groups to reflect the theme + intent. Makes the STR audit faster:

```
[Campaign: Solution] → "Project Management – Team Collaboration"
[Campaign: Competitor] → "Asana Alternative – PM Tools"
[Campaign: Problem] → "Missed Deadlines – Team Alignment"
```

Every ad group name should make it obvious what the landing page is about. If it doesn't, the structure is off.
