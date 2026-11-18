# ELUORA Meta Test Campaign Plan

**Status:** Recommendation for owner approval. Nothing has been set up, launched or spent.
**Built from:** `.agents/product-marketing.md` (v2) and the creative in this folder.
**Owner inputs (2026-11-18):** budget €20-25/day, Meta tracking tested, ships to 23 EU countries, Christmas cut-off 19 Dec. Every number that is an assumption is labelled **ASSUMPTION** and should be replaced with real figures when available.

---

## 1. The structure in one picture

```
Campaign: META_Sales_EE-FI_Broad_Test1_2026-11
Objective: Sales  ·  Conversion location: Website (eluora.co)  ·  Optimise for: Purchase
Budget: set per ad set (so each country gets a fair read)
│
├── Ad set: EE_Broad_W25-45      €12/day
│     ├── Ad 04 · The Nordic Skin Ritual (€108, ships free)
│     └── Ad 07 · The gift: THE ELUORA RITUAL (€198, ships free)
│
└── Ad set: FI_Broad_W25-45      €12/day
      └── the same 2 ads
```

**Total: €24/day** (inside your €20-25 range; €12.50 per country if you want the full €25). From a 20 November launch to 19 December that is about **€720 at most**.

## 1a. Timeline to Christmas

| Dates | Budget | What happens |
|---|---|---|
| **20 Nov** (launch) to 3 Dec | €24/day (€12 per country) | Ads 04 and 07 in both countries. Hands off for the first 3 days. |
| 27 Nov (day 7) | | Delivery check (section 7). |
| 4 Dec (day 14) | | First real decisions. Add "Order by 19 December for delivery before Christmas" to ad 07 as a **new** ad, and pause the old version. |
| 4 to 19 Dec | €24/day total | Move money toward the country with the lower cost per sale (e.g. €15 / €9). Keep the total the same. |
| **20 Dec** | €24/day | Pause ad 07. Launch ads 02 (The Purify) and 03 (The Reset) next to ad 04. |
| January | Review | Costs fall after the holidays. Decide on round 2 with what was learned. |

**Why both ritual ads first:** at €12/day per country only 2 ads get enough spend to judge. Both rituals cost over €80, so they ship free and bring the biggest orders, and gift buying peaks before 19 December. That gives the most sales value from a small budget.

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
| Daily budget | €12 | €12 |

**Why broad:** Meta's current delivery system finds buyers through the creative, not through interest lists. Your audience knowledge (women 25-45, Nordic, cares where products come from) is already written into the ads. Stacking interests on a €12/day budget would shrink the audience and raise costs.

## 4. Which concepts to test first, and why

A €12/day ad set can fairly test about **2 ads**. The rule is that each ad needs to spend at least 2× the target cost per purchase within 14 days. At a €40 target, that is (€12 × 14) ÷ (2 × €40) = 2.1 ads. Running more ads than that means none of them gets enough spend to judge.

| Wave 1 (launch, until 19 Dec) | Why it goes first |
|---|---|
| **04 · The Nordic Skin Ritual** | A full routine at €108 that ships free. Tests whether people buy the bundle straight from cold traffic. |
| **07 · The gift** | €198, the highest order value, ships free, and gift buying peaks now. Paused after the **19 December** cut-off. |

| Wave 2 | When and why |
|---|---|
| **02 · The black mask moment** | From 20 Dec, or earlier if 04 or 07 is cut. The most visual scroll-stopper. |
| **03 · Wash day reset** | From 20 Dec. The hero hair product (€42) and the everyday hair problem. |
| **06 · The Cleanse** | January. Lowest price (€28), the easiest first purchase. |
| **01 · Bog to bottle** | January. Brand story for when the account has more budget. |
| **05 · What's inside** | Better for warm audiences. Use in retargeting (section 8). |
| **08 · Review template** | **Only once you have a real review, with permission.** Retargeting only. |

**How to build each ad:**
- **One ad per concept.** Upload the 1:1 asset for Feed and the 9:16 asset for Stories and Reels in the same ad (placement asset customisation).
- **Add all 3 variations as text options.** Each concept's 3 primary texts and 3 headlines go into the ad's text options, so Meta tests the hooks inside one ad and does not split the small budget across 12 separate ads.
- **No video yet?** Launch with the 1:1 and 9:16 **stills** from each visual brief. Statics are cheaper to produce and often perform as well as video on Meta. Add the video version once a concept proves itself.

## 5. Before launch: checklist (must pass, or the test cannot be read)

- [x] Meta set up and test purchase recorded (owner, 2026-11-18)
- [ ] AddToCart, InitiateCheckout and ViewContent events firing
- [ ] eluora.co domain verified in Meta Business Manager
- [ ] Instagram @eluora.official connected to the ad account
- [x] Each ad links to the page of the product it advertises (owner confirmed). Add UTMs: `utm_source=meta&utm_medium=paid_social&utm_campaign=test1&utm_content=02-mask`
- [ ] Pages load fast on a phone inside Instagram's in-app browser (swipe up from an ad preview to check)
- [x] Ships to Estonia, Finland and the other EU countries in the store list (owner, 2026-11-18)
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
| **Day 7** | Any ad that has spent **under €21** (half its fair share of €12 ÷ 2 ads × 7 days) | Meta has decided it is weak. Pause it and launch ad 02 in its place. |
| **Day 14** | Any ad that has spent **€80 (2× target) with zero add-to-carts** | Pause it and launch the next wave 2 ad. |
| **Day 14** | Any ad with **2+ purchases** and return on ad spend of **2.5 or more** | Winner. Keep it running. |
| **Day 21** | Any ad that has spent **€120 (3× target) with zero purchases** | Pause it. |
| **Day 14 onwards** | One country clearly cheaper per purchase over the last 7 days | Move budget toward it (e.g. €15 / €9). Keep the total at €24-25. |
| **Any time** | Cost per purchase above €60 (1.5× target) for 7 days | Pause the weaker ad, or move its budget to the other country. |

**Week-by-week rhythm:** check on Monday, launch replacements on Wednesday, change budgets on Friday. Keep a one-line log of every change and its date, so a jump in results can be traced to a cause.

## 8. After the test (month 2, only if wave 1 has purchases)

1. **Scale (only if you raise the budget):** move winners into their own campaign, and keep a separate test campaign for new concepts. Keep about 80% of the money behind proven ads and 20% behind tests.
2. **Retargeting** (once the site has about 1,000 visitors from ads): website visitors from the last 30 days plus video viewers. Show them a **different** product from the one they viewed: hair viewers see the Nordic Skin Ritual, face viewers see The Scalp Reset Ritual. Use concepts 05, 06 and, once you have a real review, 08.
3. **Language test:** duplicate the best English ad in Estonian and in Finnish. Hypothesis: native-language versions get a lower cost per purchase than English, in each country. Test one country at a time.
4. **Next markets:** add one new EU country as its own ad set, using only proven ads.
5. **Log learnings** in the Learnings table in `.agents/product-marketing.md`.

## 9. Risks to know about

- **Meta's personal-attributes policy:** concept 03's first variation asks "Roots feeling heavy by day two?" Meta usually allows this for beauty, but it may be flagged as implying something about the viewer. If it is rejected, drop it and keep variations 2 and 3.
- **Packaging text:** labels showing "Detoxifying", "Antibacterial" or "Natural" in the creative can trigger a review against your own rules (and some markets' cosmetics claim rules). Frame them out.
- **Q4 costs:** November and December ad prices are the highest of the year. A January re-test will likely be cheaper; do not read a weak December as a weak product.
- **Small sample:** at €24/day, expect a handful of purchases per concept, not hundreds. Treat the winners as strong candidates to keep testing, not proven facts.

---

## Facts, assumptions and missing data

**Facts (from the catalogue, the price list and the owner):** product range and prices, EE and FI first, women 25-45, English ads, no reviews yet, the gift bundle includes the black case.

**Assumptions (replace when known):**
- €24/day budget (owner range €20-25)
- €40 target cost per purchase (40% margin on a €100 average order)
- Purchase tracking will be working before launch

**MISSING (needed to judge results properly):**
- Gross margin per product and average order value → real break-even cost per purchase
- Any past sales or ad data (best seller)

**Approval needed before any spend:** I will not create the campaign, upload ads, or use image or video tools. When you are ready, confirm the budget and I can turn this into a step-by-step Ads Manager setup sheet.
