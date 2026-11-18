# ELUORA Meta Test Campaign Plan

**Status:** Recommendation for owner approval. Nothing has been set up, launched or spent.
**Built from:** `.agents/product-marketing.md` (v2) and the creative in this folder.
**Owner instruction:** budget and tracking not supplied; "use what you recommend for maximum outcome." Every number that is an assumption is labelled **ASSUMPTION** and should be replaced with real figures when available.

---

## 1. The structure in one picture

```
Campaign: META_Sales_EE-FI_Broad_Test1_2026-11
Objective: Sales  ·  Conversion location: Website (eluora.co)  ·  Optimise for: Purchase
Budget: set per ad set (so each country gets a fair read)
│
├── Ad set: EE_Broad_W25-45      €20/day
│     ├── Ad 02 · The black mask moment (The Purify)
│     ├── Ad 03 · Wash day reset (The Reset)
│     ├── Ad 04 · The Nordic Skin Ritual (€108)
│     └── Ad 07 · The gift: THE ELUORA RITUAL (€198)
│
└── Ad set: FI_Broad_W25-45      €20/day
      └── the same 4 ads
```

**Total:** €40/day (top of your €20-40 range). See the timeline in section 1a: about **€1,200 maximum** from launch to 19 December, and never more than €40 on any day.
**Lean option:** €10/day per country (€20/day, ≈ €420 for 21 days). At that budget only **2 ads per country** get enough spend to judge, so launch just 04 (Nordic Skin Ritual) and 07 (the gift) and wait the full 21 days before deciding.


## 1a. Timeline to Christmas

| Dates | Budget | What happens |
|---|---|---|
| **Launch as soon as the test order works** (aim for 20 Nov) to 3 Dec | €40/day (€20 per country) | Wave 1: ads 02, 03, 04 and 07 in both countries. Hands off for the first 3 days. |
| 4 Dec (day 14) | | First decisions (section 7): cut weak ads, swap in wave 2. |
| 4 to 19 Dec | Up to €40/day total | Shift money toward the stronger country and the winning ads. Add the line "Order by 19 December for delivery before Christmas" to ad 07 as a new ad. Do not go above €40/day; at this budget there is no step up to make. |
| **20 Dec** | Drop to €20/day | Pause ad 07 and remove any Christmas lines. Keep running the winners; add 06 (The Cleanse) and 01 (Bog to bottle). |
| January | Review | Costs fall after the holidays. Re-test with what was learned. |

**If you prefer €20/day:** run €10 per country with only ads 04 and 07 until 19 December, then switch to 02 and 03.

**Free shipping over €80 helps:** both rituals (€108, €198) ship free, single products do not. Expect the ritual ads to have a higher order value; judge them on return on ad spend, not only on cost per purchase.

## 2. Campaign settings

| Setting | Recommendation | Why |
|---|---|---|
| Objective | **Sales** | You want purchases, so Meta should look for buyers, not clickers. |
| Performance goal | Maximise number of conversions, event **Purchase** | Fallback: if the pixel has not yet recorded any purchases, optimise for **Add to cart** for the first 2 weeks, then switch to Purchase in a new campaign. |
| Budget type | **Ad set budget** (Advantage campaign budget off) | With a campaign budget, Meta can send almost all money to one country, and you would learn nothing about the other. |
| Bid strategy | Highest volume (no cap) | Caps need conversion history you do not have yet. |
| Attribution | 7-day click, 1-day view (Meta default) | Keep it the same for the whole test so results are comparable. |
| Name | `META_Sales_EE-FI_Broad_Test1_2026-11` | Platform, objective, market, audience, test, month. |

## 3. Ad set settings (one per country)

| Setting | Estonia ad set | Finland ad set |
|---|---|---|
| Name | `EE_Broad_W25-45` | `FI_Broad_W25-45` |
| Location | Estonia, people living in this location | Finland, people living in this location |
| Audience | **Advantage+ audience on**, with suggestion: women 25-45. Hard minimum age 25. No interests. | Same |
| Language | Leave empty (ads are in English) | Same |
| Placements | Advantage+ placements (Feed, Stories, Reels, etc.) | Same |
| Exclusions | Purchasers in the last 180 days (once the pixel has data) | Same |
| Daily budget | €20 | €20 |

**Why broad:** Meta's current delivery system finds buyers through the creative, not through interest lists. Your audience knowledge (women 25-45, Nordic, cares where products come from) is already written into the ads. Stacking interests on a €20/day budget would shrink the audience and raise costs.

## 4. Which concepts to test first, and why

A €20/day ad set can fairly test about **4 ads**. The rule is that each ad needs to spend at least 2× the target cost per purchase within 14 days. At a €40 target, that is (€20 × 14) ÷ (2 × €40) = 3.5 ads. Running more ads than that means none of them gets enough spend to judge.

| Wave 1 (launch) | Why it goes first |
|---|---|
| **02 · The black mask moment** | The most visual scroll-stopper. It tests whether the peat texture earns attention in a beauty feed. |
| **03 · Wash day reset** | The clearest everyday problem (heavy roots and build-up) with the hero hair product at €42. It tests the scalp and hair side of the brand. |
| **04 · The Nordic Skin Ritual** | A full routine at €108. It tests whether people buy the bundle straight from cold traffic. |
| **07 · The gift** | Gift buying peaks now, €198 is the highest order value, and it ships free (over €80). Runs until the **19 December** order cut-off, then is paused. |

| Wave 2 (swap in as ads are cut, from week 2) | Use |
|---|---|
| **01 · Bog to bottle** | Brand story. The first replacement if 02 or 03 is cut. |
| **06 · The Cleanse** | Lowest price (€28), the easiest first purchase. Replaces 07 after the gift window. |
| **05 · What's inside** | Better for warm audiences. Use in retargeting (section 8). |
| **08 · Review template** | **Only once you have a real review, with permission.** Retargeting only. |

**How to build each ad:**
- **One ad per concept.** Upload the 1:1 asset for Feed and the 9:16 asset for Stories and Reels in the same ad (placement asset customisation).
- **Add all 3 variations as text options.** Each concept's 3 primary texts and 3 headlines go into the ad's text options, so Meta tests the hooks inside one ad and does not split the small budget across 12 separate ads.
- **No video yet?** Launch with the 1:1 and 9:16 **stills** from each visual brief. Statics are cheaper to produce and often perform as well as video on Meta. Add the video version once a concept proves itself.

## 5. Before launch: checklist (must pass, or the test cannot be read)

- [x] Meta set up (owner, 2026-11-18). Still do **one real test order** and check Events Manager shows Purchase with `value` and `currency: EUR`, then refund it
- [ ] AddToCart, InitiateCheckout and ViewContent events firing
- [ ] eluora.co domain verified in Meta Business Manager
- [ ] Instagram @eluora.official connected to the ad account
- [x] Each ad links to the page of the product it advertises (owner confirmed). Add UTMs: `utm_source=meta&utm_medium=paid_social&utm_campaign=test1&utm_content=02-mask`
- [ ] Pages load fast on a phone inside Instagram's in-app browser (swipe up from an ad preview to check)
- [ ] Finland is switched on as a shipping country in the store (the country list sent on 18 Nov showed only Estonia ticked)
- [ ] "Free shipping over €80" and "Order by 19 December for Christmas delivery" visible on product pages and at checkout
- [ ] Footage and stills reviewed for legible banned words on packaging (see `README.md`)

## 6. The numbers to watch

**Target cost per purchase: €40 (ASSUMPTION).** I worked this backwards from typical beauty margins and the €108 ritual price. Replace it with your real number using:

> **Break-even cost per purchase = average order value × gross margin %**
> Example (ASSUMPTION): €100 average order × 40% margin = €40. Above that, each sale loses money on the first order.

| Stage | Metric | Where in Ads Manager | Healthy sign (starting point, recalibrate after 14 days) | What a bad number means |
|---|---|---|---|---|
| Attention | **Hook rate** = 3-second video plays ÷ impressions (video only) | Custom column | 25% or more | The first 2 seconds do not stop the scroll. Change the hook or opening shot. |
| Attention | **CPM** (cost per 1,000 impressions) | Default | Stable or falling week to week | Rising CPM is the earliest sign of fatigue. Q4 CPMs run high in all markets. |
| Interest | **Link CTR** | Default | 1% or more | The ad does not make people want to know more. Test a different variation or concept. |
| Interest | **Cost per landing page view** | Default | Falling as Meta learns | |
| Interest | **Landing page views ÷ link clicks** | Calculated | 70% or more | Under 70% usually means a slow page or broken link. |
| Intent | **Add-to-cart rate** = add to carts ÷ landing page views | Calculated | Watch for the trend | Clicks with no add-to-carts mean the page or price does not match what the ad promised. |
| Result | **Purchases** and **cost per purchase** | Default | ≤ €40 (target) | |
| Result | **ROAS** = purchase value ÷ spend | Default | At least 2.5 (≈ break-even on a €100 order at €40 cost per purchase) | |
| Result | **Average order value** | Purchase value ÷ purchases | Higher on 04 and 07 | Shows whether the rituals pull up basket size. |
| Health | **Frequency** | Default | Under 2.5 for this cold campaign | Over 3 means the same people keep seeing it. Add fresh creative. |
| Market | **Cost per purchase EE vs FI** | Breakdown | | Decides where the budget goes in month 2. |

## 7. Decision rules (when to act, and when to wait)

Never edit a running ad: editing restarts Meta's learning. Pause it and launch a replacement instead. Pausing does not restart learning.

| When | Check | Action |
|---|---|---|
| **Days 1-3** | Are purchases and add-to-carts being recorded? Is every ad spending? | Change nothing else. Results in the first 72 hours are noise. |
| **Day 7** | Any ad that has spent **under €17.50** (half its fair share of €20 ÷ 4 ads × 7 days) | Meta has decided it is weak. Pause it and launch a wave 2 concept in its place. |
| **Day 7+** | Any ad that has spent **€80 (2× target) with zero add-to-carts** | Pause it. |
| **Day 14** | Any ad that has spent **€120 (3× target) with zero purchases** | Pause it. Replace with the next wave 2 concept. |
| **Day 14** | Any ad with **3+ purchases at ≤ €40 each** | Winner. Keep it running. Make 2 new versions of its hook for the next round. |
| **Every 4-5 days after day 14** | Ad set cost per purchase ≤ €40 over the last 7 days, frequency under 2.5 | Raise that ad set's budget by **20%**, never more in one step. |
| **Any time** | Cost per purchase above €60 (1.5× target) for 7 days after a budget increase | Cut the budget back by 20-30% and hold for a week. |
| **Day 21** | Compare countries and concepts | Move budget to the stronger country. Retire losers. Plan round 2 around the winning concept. |

**Week-by-week rhythm:** check on Monday, launch replacements on Wednesday, change budgets on Friday. Keep a one-line log of every change and its date, so a jump in results can be traced to a cause.

## 8. After the test (month 2, only if wave 1 has purchases)

1. **Scale:** move winners into their own campaign, and keep a separate €8-10/day test campaign for new concepts. Keep about 80% of the money behind proven ads and 20% behind tests.
2. **Retargeting** (once the site has about 1,000 visitors from ads): website visitors from the last 30 days plus video viewers. Show them a **different** product from the one they viewed: hair viewers see the Nordic Skin Ritual, face viewers see The Scalp Reset Ritual. Use concepts 05, 06 and, once you have a real review, 08.
3. **Language test:** duplicate the best English ad in Estonian and in Finnish. Hypothesis: native-language versions get a lower cost per purchase than English, in each country. Test one country at a time.
4. **Next markets:** add one new EU country as its own ad set, using only proven ads.
5. **Log learnings** in the Learnings table in `.agents/product-marketing.md`.

## 9. Risks to know about

- **Meta's personal-attributes policy:** concept 03's first variation asks "Roots feeling heavy by day two?" Meta usually allows this for beauty, but it may be flagged as implying something about the viewer. If it is rejected, drop it and keep variations 2 and 3.
- **Packaging text:** labels showing "Detoxifying", "Antibacterial" or "Natural" in the creative can trigger a review against your own rules (and some markets' cosmetics claim rules). Frame them out.
- **Q4 costs:** November and December ad prices are the highest of the year. A January re-test will likely be cheaper; do not read a weak December as a weak product.
- **Small sample:** at €40/day, expect a handful of purchases per concept, not hundreds. Treat the winners as strong candidates to keep testing, not proven facts.

---

## Facts, assumptions and missing data

**Facts (from the catalogue, the price list and the owner):** product range and prices, EE and FI first, women 25-45, English ads, no reviews yet, the gift bundle includes the black case.

**Assumptions (replace when known):**
- €40/day budget within the owner's €20-40 range
- €40 target cost per purchase (40% margin on a €100 average order)
- Purchase tracking will be working before launch

**MISSING (needed to judge results properly):**
- Gross margin per product and average order value → real break-even cost per purchase
- Any past sales or ad data (best seller)

**Approval needed before any spend:** I will not create the campaign, upload ads, or use image or video tools. When you are ready, confirm the budget and I can turn this into a step-by-step Ads Manager setup sheet.
