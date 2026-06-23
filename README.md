# TechHaven - E-commerce Analysis

TechHaven is a global e-commerce company founded in 2018 specializing in consumer
electronics. This analysis covers **$28M in revenue across 108K orders from 2019–2022**,
examining product trends, refunds, loyalty program performance, and marketing channels.

---

# Executive Summary

<div align="center">
  <img src="images/sales_trends.png" width="80%">
</div>

TechHaven rode the pandemic wave to peak performance in 2020–2021, but the underlying
business has structural weaknesses — product concentration, a loyalty program that
enrolls without retaining, and marketing channels that haven't diversified beyond
organic traffic — now exposed as external tailwinds fade.

- **$28M in total revenue**, 108K orders, $260 AOV across 2019–2022
- **Pandemic peak (Mar 2020–Mar 2021):** $12M in sales, $297 AOV, 39K orders
- **Post-normalization (Jan 2022+):** Revenue fell to $4M, AOV declined to $229
- **Gaming Monitor, AirPods, and MacBook** account for ~82% of total revenue
- **Loyalty program is not driving retention** — only 39 of 38,756 members made repeat purchases
- **Email is the only channel** to grow in both 2020 (+223%) and 2021 (+24%)
- **⚠️ 2022 refund data missing** — likely a data integrity issue requiring validation

---

# Analysis & Insights

## Product Trends & Apple Spotlight

Three products drive 82% of TechHaven's revenue with ~97% concentrated among a
handful of brands — a concentration risk that compounds as Apple, once the category
leader, has declined since Q4 2021. Gaming Monitor has grown its share steadily to
fill the gap, while Bose Headphones and Samsung Webcam show trends too limited or situational
to rely on going forward.

### Performance by Period

| Period | Total Sales | AOV | Total Orders |
|---|---|---|---|
| 2019–2022 (Full) | $28M | $260 | 108K |
| Jan 2019–Mar 2020 (Pre-Pandemic) | $5M | $237 | 20K |
| Mar 2020–Mar 2021 (Pandemic Peak) | $12M | $297 | 39K |
| Mar 2021–Jan 2022 (Post-Pandemic) | $7M | $246 | 30K |
| Jan 2022+ (Normalization) | $4M | $229 | 19K |

### Top 3 Product Share

Revenue and order leadership tell different stories — Gaming Monitor leads in dollars
while AirPods dominate by volume. Samsung Charging Cable ranks 3rd in orders but
barely registers in revenue, illustrating the gap between what drives transactions
and what drives the business.

<div align="center">
  <img src="images/Top3 - 4K Gaming Monitor Leads Top 3 Products in Revenue.png" width="45%">
  <img src="images/Top3 - Airpods Lead Top 3 Products by Order in Total Orders.png" width="45%">
</div>

- **Revenue leaders:** Gaming Monitor ($9.8M), AirPods ($7.7M), MacBook ($6.3M) — 82% of total
- **Order leaders:** AirPods (48K), Gaming Monitor (23K), Samsung Charging Cable (22K)
- **Samsung Charging Cable:** 22K orders but only $442K revenue — $20 AOV
- **Gaming Monitor revenue share** grown from ~35% to 50%+ by late 2022
- **MacBook revenue share eroding** since Q4 2021, absorbed by Gaming Monitor
- **~97% of revenue** concentrated among Apple, Lenovo, and a small group of brands
- **Bose:** -91% decline in 2022 across only 27 total orders — not enough data to conclude
- **Samsung Webcam:** +134% in 2021 driven by remote work demand — unlikely to sustain

### Gaming Monitor by Region

Gaming Monitor is the top product in every region, with North America leading by a
significant margin. Outside of NA and EMEA, contribution remains minimal.

<div align="center">
  <img src="images/Top3 - 4K Gaming Monitor Overtakes Macbook in all Regions.png" width="80%">
</div>

- **Most popular product across all regions** — NA leads at nearly 3x EMEA
- **NA peaked at ~$186K** monthly in Jan 2022; late-2022 uptick worth monitoring
- **LATAM and APAC** remain minimal contributors throughout the period

### Apple Spotlight

Apple peaked in late 2020 and has declined across all regions since Q4 2021. MacBook's
sales and order volume move in lockstep — this is a demand problem, not a pricing or
product mix issue.

<div align="center">
  <img src="images/Macbook North American AoV Fluctuates with 4Q22 Outlier.png" width="70%">
</div>

- **Apple peaked Sep–Dec 2020**, declining in all regions since Q4 2021
- **MacBook sales and volume in lockstep** — volume problem, not a pricing issue
- **Q4 2022 MacBook AOV dropped to ~$1,200** from a typical $1,500–$1,700 — investigate
- **AirPods:** 48K orders at $160 AOV — most consistent and predictable volume driver
- Apple refunds outpace all other brands — see [Refunds](#refunds) for full breakdown

### Pricing Anomalies

Several products show orders at price ranges inconsistent with known retail pricing.
These are flagged for data integrity review and should be noted in any AOV or revenue
analysis.

| Product | Suspicious Price Range | Order Count | AOV |
|---|---|---|---|
| 27in 4K Gaming Monitor | $1–$100 | 73 | $421 |
| Apple AirPods | $1–$50 | 183 | $160 |
| MacBook Air Laptop | $1–$1,000 | 259 | $1,591 |
| Samsung Charging Cable Pack | $1,000+ | 1 | $20 |
| ThinkPad Laptop | <$1,000 | 550 | $1,101 |

- **ThinkPad and MacBook** carry the largest risk — 550 and 259 orders at prices well below retail
- **Samsung Charging Cable's** single $1,000+ order is likely a data entry error

---

## Refunds

MacBook generates the highest total refund dollar impact despite not having the most
refunds — its $1,588 AOV makes each return disproportionately costly. A 2022 data gap
prevents trend conclusions and needs to be resolved before drawing year-over-year
comparisons.

<div align="center">
  <img src="images/Reunds - Treemap.png" width="45%">
  <img src="images/Refunds - Total Avg.png" width="50%">
</div>

- **MacBook:** Highest total refund value at $717K (452 refunds, 11% rate, $1,588 AOV)
- **Gaming Monitor:** $608K total refund value (1,445 refunds, 6% rate)
- **AirPods:** $421K — 3rd despite most refunds (2,636) due to lower $160 AOV
- **ThinkPad:** Highest refund rate at 12% but 4th in total impact ($377K, 343 refunds)
- **Rate alone is misleading** — AOV and volume must be considered together
- **Apple:** 58% of all refunds (3,110) at 6% avg rate — driven by AirPods volume
- **Lenovo:** 12% rate | **Samsung:** 2% rate | **Bose:** 0% across 27 orders (unreliable)
- **Premium tier:** Highest blended refund rate at 7% across ~4K refunds
- **2020 spike:** AirPods generated ~1,550 refunds — nearly double 2019 volume
- **⚠️ 2022 data flag:** 0 refunds recorded despite 21,565 orders — ~1,000+ expected
- **Loyalty members:** 2.8K refunds vs. non-loyalty 2.5K despite fewer total orders
- **Non-loyalty refund AOV:** ~$549 vs. loyalty ~$297 — converging to ~$225 by 2022

*Refund behavior by loyalty segment raises broader questions about program effectiveness —
see [Loyalty Program Performance](#loyalty-program-performance) below.*

---

## Loyalty Program Performance

The loyalty program has grown to 38,756 members and surpassed non-loyalty in total
sales since Q2 2021 — but those numbers obscure a critical problem. Only 39 members
have ever made more than one purchase, pointing to a program that signs customers up
without changing their behavior.

<div align="center">
  <img src="images/39 Returning Loyalty Members; $29K Total Sales.png" width="80%">
</div>

<div align="center">
  <img src="images/Loyalty Program AoV2.png" width="45%">
  <img src="images/Loyalty Program Total Sales Outpace Non Members 2Q-2021 but Falter Q4-2022.png" width="45%">
</div>

- **38,756 loyalty members vs. 48,842 non-loyalty** across the period
- **Non-loyalty generated ~$17M vs. loyalty ~$11M** across the full period
- **Loyalty overtook non-loyalty in sales from Q2 2021** — non-loyalty pulled back ahead in Q4 2022
- **⚠️ 0% effective repeat rate** — only 39 of 38,756 members purchased on multiple dates
- **$29K in repeat sales** from returning members — enrolling but not retaining
- **Loyalty AOV flat** (~$220–$260) throughout — the crossover reflects non-loyalty decline,
  not loyalty strength
- **Non-loyalty AOV spiked to ~$380** in 2020 then crashed back, overtaking loyalty by Q4 2022
- **Loyalty members refund more** (2.8K vs. 2.5K) despite fewer total orders

<div align="center">
  <img src="images/Loyalty - Loyalty Members Return More Often2.png" width="50%">
</div>

**Verdict:** With a 0% repeat rate, higher refund frequency, and eroding performance
advantages by Q4 2022, the program requires significant restructuring. The more pressing
question is whether the program is profitable at all — if members are signing up once
for a discount on a largely single-purchase product category and never returning, the
program may be losing money rather than driving growth.

---

## Marketing Channel Performance

Email is the only managed channel that sustained growth beyond the pandemic and is
the primary touchpoint for loyalty members. Every other channel declined in 2021,
making Email the clearest lever for retention and acquisition investment.

![Marketing Channel Chart](images/marketing_channel.png)

- **Email only channel to grow in both 2020 (+223%) and 2021 (+24%)**
- **Email is the primary loyalty channel** — only channel where loyalty leads non-loyalty (11K vs. 8K)
- **Direct dominates at $23M (~82%)** — organic behavior, not a managed channel
- **Affiliate has the highest AOV** at ~$303 despite only 2,900 orders — underinvested
- **Social Media:** Highest refund rate at 7.58% despite only 1,293 orders
- **Unknown channel:** Spiked +2,325% in 2020 and +295% in 2022 — likely attribution error

| Channel | Order Count | Refund Rate | 2020 YoY | 2021 YoY |
|---|---|---|---|---|
| Email | 18,553 | 4.76% | +222.60% | +24.46% |
| Direct | 83,884 | 5.03% | +160.59% | -12.70% |
| Affiliate | 2,900 | 4.76% | +86.36% | -41.29% |
| Social Media | 1,293 | 7.58% | +95.02% | -21.32% |
| Unknown | 1,469 | 2.45% | +2,324.56% | -12.32% |

---
## Regional Performance

All four regions followed the same pandemic-driven arc — spike in 2020, peak in 2021,
contraction in 2022 — with NA and EMEA driving the overwhelming majority of revenue
throughout. The pattern was global, not market-specific.

<div align="center">
  <img src="images/regional_brand.png" width="45%">
  <img src="images/sales_region.png" width="45%">
</div>

- **NA ~54% of revenue ($14M)**, EMEA ~30% ($8M) — together over 80% of total
- **All four regions mirrored the same growth and decline pattern** — 2020 pandemic
  spike, 2021 peak, 2022 contraction were global in nature, not driven by any single market
- **NA deviated slightly** — smaller decline in 2021 (-16%) vs. other regions, followed
  by a steeper drop in 2022 (-39%)
- **November and December are peak months across NA, EMEA, and APAC** — consistent
  holiday-driven demand that can be planned around. LATAM breaks from this pattern,
  peaking in July (+24%) rather than the holiday season, with a more modest Nov–Dec
  lift (~10%) — suggesting distinct regional demand drivers that warrant a tailored
  approach rather than a global campaign strategy
- **NA accounts for ~$1.2M in total refunds** — more than double EMEA at $569K,
  making it the primary driver of refund-related financial impact
---

| Priority | Department | Recommendation |
|---|---|---|
| 🔴 High | **Product** | Investigate Apple's steep 2022 decline — root cause analysis needed |
| 🔴 High | **Product** | Resolve pricing anomalies flagged across 5 products |
| 🔴 High | **CRM** | Restructure loyalty program — 0% repeat rate indicates fundamental retention failure |
| 🔴 High | **CRM** | Audit purchase history of loyalty members — low repeat rate and single-purchase product nature suggest members may be signing up for a one-time discount with no intent to return |
| 🔴 High | **CRM** | Evaluate profitability of loyalty member sign-ups — if acquisition costs are not recovered through repeat purchases, the program's net value may be negative |
| 🔴 High | **Marketing** | Invest in Email — only channel growing in both 2020 and 2021; primary loyalty touchpoint |
| 🟡 Medium | **Sales** | Expand brand portfolio to reduce ~97% revenue concentration risk |
| 🟡 Medium | **CRM** | Introduce loyalty member benefits to drive engagement — e.g. exclusive offers, shipping perks, or early product access |
| 🟡 Medium | **Marketing** | Resolve Unknown channel attribution anomaly before drawing channel-level conclusions |
| 🟢 Low | **Sales** | Promote Samsung Charging Cables alongside higher-value purchases to increase basket size |
| 🟢 Low | **Product** | Evaluate Bose product line viability — 27 total orders over 4 years |
| 🟢 Low | **Data** | Validate 2022 refund data — 0 refunds across 21,565 orders is likely an error |
