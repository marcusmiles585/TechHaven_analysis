# **TechHaven_analysis**
Sales trends analysis for e-commerce company

---

## 🚀 **Overview**
TechHaven is an e-commerce company founded in 2018, specializing in popular consumer electronics. With a strong global presence across both their website and mobile app, they have grown into a $28M business offering products from top brands including Apple, Samsung, Bose, and Lenovo.

TechHaven's Head of Operations has requested a comprehensive analysis of company performance between 2019 and 2022. This analysis addresses key business questions across sales trends, product performance, regional insights, customer loyalty, and operational efficiency — providing actionable insights and recommendations to support sustained growth.

This analysis covers five key areas of TechHaven's business performance.

***Sales Trends***: Examines year-over-year and month-over-month growth patterns, including seasonality drivers.\
***Product Performance***: Identifies top and bottom performers across product lines, with a focus on refund rates and revenue concentration.\
***Regional Performance***: Explores how products perform across global markets and highlights emerging growth opportunities.\
***Loyalty Program Performance***: Evaluates the effectiveness of the loyalty program and whether continued investment is warranted.\
***Marketing Channel Performance***: Analyzes how each acquisition channel contributes to order volume, revenue, and customer quality.


## **Recommendations**

<table>
  <tr>
    <th>Department</th>
    <th>Recommendations</th>
  </tr>

  <tr>
    <td><strong>Sales</strong></td>
    <td>
      • Use high‑volume, lower‑value items as upsell levers<br>
      • Expand brand portfolio to reduce dependency concentration<br>
      • Verify low sales for Bose in 2022 as being accurate and not an error
    </td>
  </tr>

  <tr>
    <td><strong>Product</strong></td>
    <td>
      • Expand Samsung portfolio as strong Post Pandemic performance<br>
      • Investigate and evaluate Bose product line<br>
      • Investigate pricing outliers and discount leakage<br>
      • Improve product content to reduce return rates
    </td>
  </tr>

  <tr>
    <td><strong>CRM</strong></td>
    <td>
      • Sustain and expand the loyalty program<br>
      • Introduce tiered loyalty benefits to drive higher spending<br>
      • Develop win‑back campaigns for lapsed non‑loyalty customers<br>
      • Audit “Unknown” channel attribution
    </td>
  </tr>

  <tr>
    <td><strong>Marketing</strong></td>
    <td>
      • Prioritize high‑revenue and high‑volume products<br>
      • Optimize campaigns by region & seasonality<br>
      • Scale affiliate channel<br>
      • Audit “Unknown” channel attribution
    </td>
  </tr>

</table>



## **Anaysis & Insights**

### <ins>Sales Trends<ins>
*TechHaven generated $28M in total revenue between 2019 and 2022, with growth peaking in 2021 
before a broad market contraction in 2022 brought performance closer to pre-pandemic baselines.*

![Sales Trends Chart](images/sales_trends.png)

- **Overall Revenue & Regional Distribution:** North America was the dominant market, 
contributing ~52% of total revenue ($14M), followed by EMEA at ~29% ($8M). Sales remain 
heavily concentrated in these two regions, with other markets representing a relatively 
small share of total volume.

- **Year-over-Year Growth:** 2020 saw a significant spike in both order volume (+101%) and 
sales, largely driven by pandemic-related demand. Growth peaked in 2021 before declining 
sharply in 2022 (-40% in order volume), though 2022 figures still remained above pre-pandemic 
2019 levels.

- **Month-over-Month Seasonality:** Performance consistently dips in September–October and 
again in February, before rebounding in March and peaking during the November–December holiday 
period. These seasonal patterns held across nearly every year in the dataset.

- **2022 Contraction:** October 2022 marked the sharpest single-month decline in the dataset, 
with total sales falling -55%, AOV dropping -16%, and order count declining -47%. This 
contraction was broad-based, affecting all regions and product categories simultaneously.

- **AOV Stability:** Despite significant swings in order volume and total sales, Average Order 
Value remained relatively stable throughout the period. Notably, AOV dipped in November — 
suggesting holiday-driven volume was fueled by lower-priced items or promotions rather than 
higher-value purchases.


### <ins>Product Performance<ins>
*A small number of products drive the vast majority of TechHaven's revenue and order volume, 
while high-AOV items like ThinkPad and MacBook carry disproportionate financial risk 
from refunds.*

<div align="center">
  <img src="images/sales_brand.png" width="30%">
  <img src="images/sales_region.png" width="30%">
</div>

- **Top Performers by Revenue:** Gaming Monitor led all products at $9.8M in total revenue, 
followed by AirPods at $7.7M and MacBook at $6.2M. Together these three products account 
for the majority of TechHaven's total revenue, indicating a high concentration risk across 
the portfolio.

- **Top Performers by Order Volume:** AirPods dominated order share at ~45% of total orders, 
followed by Gaming Monitors at 22% and Samsung Charging Cables at 20%. Collectively these 
three products represent ~87% of all orders placed across the four-year period.

- **Brand Concentration:** Apple, Lenovo, and a small group of key brands collectively account 
for ~97% of total revenue. While these brands are clearly resonating with customers, this 
level of concentration presents a dependency risk if any one brand relationship were to change.

- **Declining & At-Risk Products:** Bose experienced a -91% decline in 2022 and had only 27 
total orders over four years, making it difficult to draw meaningful conclusions from its 0% 
refund rate. Samsung Webcams saw exceptional growth in 2021 (+134%) driven by remote work 
demand, though this trend is unlikely to sustain as the market normalizes.

- **Refund Performance:** High-AOV products like ThinkPad and MacBook carry disproportionate
financial risk from returns, while high-volume products like AirPods and Gaming Monitors
present operational risk at scale. See the [Refunds](#refunds) section for a full breakdown.

## Product Trends & Apple Spotlight

*Three products dominate TechHaven's revenue and order share across all four years, while
Apple — once the clear category leader - has seen continued decline since Q4 2021,
warranting deeper investigation into the steep 2022 drop-off.*

### Performance by Period
| Period | Total Sales | AOV | Total Orders |
|---|---|---|---|
| 2019–2022 (Full) | $28M | $260 | 108K |
| Jan 2019–Mar 2020 (Pre-Pandemic) | $5M | $237 | 20K |
| Mar 2020–Mar 2021 (Pandemic Peak) | $12M | $297 | 39K |
| Mar 2021–Jan 2022 (Normalization) | $7M | $246 | 30K |
| Jan 2022+ (Post-Normalization) | $4M | $229 | 19K |

The pandemic window (Mar 2020–Mar 2021) was the clear performance peak across all
three metrics — $12M in sales, $297 AOV, and 39K orders. Each subsequent period has
seen declining sales, AOV, and order volume, with the post-normalization period
returning closer to pre-pandemic baselines at $4M and $229 AOV.

### Pricing Anomalies

The following products show orders at price ranges inconsistent with their known
retail pricing. These records have been flagged for data integrity review and should
be noted in any pricing or AOV analysis.

| Product | Suspicious Price Range | Order Count |AOV
|---|---|---|---
| 27in 4K Gaming Monitor | $1–100 | 73 | $421 |
| Apple AirPods | $1–50 | 183 | $160 |
| MacBook Air Laptop | $1–1000 | 259 | $1,591 | 
| Samsung Charging Cable Pack | $1,000+ | 1 | $20 |
| Thinkpad Laptop | <$1,000 | 550 | $1,101 |

ThinkPad and MacBook represent the largest anomaly risk by order count — 550 and
259 orders respectively at price points well below retail. At their AOVs of $1,101
and $1,591, even a small number of mispriced orders could meaningfully skew revenue
and AOV figures. The Samsung Charging Cable Pack's single $1,000+ order is likely
a data entry error given its $20 AOV.

### Top 3 Product Share

<div align="center">
  <img src="images/top3_revenue_share.png" width="45%">
  <img src="images/top3_order_share.png" width="45%">
</div>

- **Three Products Dominate:** By revenue, the 27in 4K Gaming Monitor ($9.8M), Apple
AirPods ($7.7M), and MacBook Air ($6.3M) account for the vast majority of
TechHaven's total revenue across the period. Together, these three products represent
an overwhelming share of the $28M total ($23M) - indicating significant portfolio
concentration risk. By order count, AirPods (48,391), Gaming Monitor (23,404), and
Samsung Charging Cable (21,912) lead; with Samsung Charging Cable contributing only
$442K in revenue despite its high order volume, reflecting its $20 AOV

- **Gaming Monitor Grows Revenue Share:** On the revenue side, Gaming Monitor has
grown from ~35% to nearly 50%+ share by late 2022, largely absorbing MacBook's decline.

### Gaming Monitor by Region

<div align="center">
  <img src="images/gaming_monitor_region.png" width="75%">
</div>

- **Gaming Monitor is the Most Popular Product Across All Regions:** North America
leads Gaming Monitor sales by a significant margin - nearly 3x EMEA, the second
largest market - peaking at ~$186K in Jan 2022 before normalizing. All
regions follow the same general pandemic spike and normalization pattern, though NA
shows the sharpest volatility with a notable late 2022 uptick suggesting potential
renewed demand worth monitoring.

- **LATAM and APAC Remain Minimal Contributors:** Despite Gaming Monitor's global
dominance, LATAM and APAC contribute minimally to its overall revenue. LATAM in
particular remains flat throughout the entire period, suggesting either limited
market penetration or low purchasing power relative to the product's price point.

### Apple Spotlight

<div align="center">
  <img src="images/apple_dashboard.png" width="100%">
</div>

- **Apple Peak Late 2020, Declining Steadily Since:** North America drove
the majority of Apple's pandemic-era growth, peaking between September and December
2020. All regions have declined since Q4 2021, with the rate of decline steepening
notably through 2022. The cause of this steep drop-off warrants
further investigation before drawing permanent conclusions about Apple's trajectory.

- **MacBook NA Sales and Volume Move in Lockstep:** MacBook sales and order volume
in North America track extremely closely throughout the period, Both metrics peaked in
late 2020 at ~$149K and ~95 orders respectively, and have declined in parallel since -
pointing to a volume problem rather than a pricing or mix problem.

- **MacBook AOV Shows a Notable Q4 2022 Outlier:** MacBook AOV in North America
has fluctuated across the period, typically fluctuating in the $1,500 –
$1,700 range. However, Q4 2022 shows a sharp drop to approximately $1,200 — well
below the historical range. This could indicate heavy discounting, a pricing error,
or a data integrity issue and should be investigated before citing this figure in
executive reporting.

- **MacBook Revenue Share Eroding:** MacBook's share of revenue has been on the
decline since late 2022. This aligns with the broader Apple decline and is not
reflected in order counts since MacBook never led on volume.

- **AirPods: High Volume, Moderate AOV:** AirPods lead all products in order
count at 48K but carry an AOV of only $160. Their order share has remained remarkably
consistent, making them the most predictable volume driver in the portfolio.

- **Apple Refunds Outpace All Other Brands:** Apple consistently generates the
highest refund volume of any brand, with counts growing through the pandemic peak
before declining alongside overall sales. See the [Refund Trends](#refund-trends) section
for a full product and brand-level breakdown.


## Refunds

*Refund risk at TechHaven splits into two distinct categories - high volume concentrated
in Apple products and high rate concentrated in Lenov - though a likely
2022 data integrity issue means trends should be interpreted with caution.*

<div align="center">
  <img src="images/refund_brand_share.png" width="45%">
  <img src="images/refund_treemap.png" width="45%">
</div>

- **Refund Rate vs. Refund Volume:** ThinkPad carries the highest refund rate at 12% but
only 343 total refunds, while AirPods account for 21% of all refunds at 2,636 — the
highest by volume. The top 3 by refund rate are ThinkPad (12%, 343 refunds), MacBook (11%,
453 refunds), and Apple iPhone (8%, 22 refunds). The top 3 by refund count are AirPods
(2,636), Gaming Monitor (1,445), and MacBook (453).

- **Apple Dominates Refund Volume Despite Average Rate:** Apple accounts for 58% of
all refunds (3,110 total) despite carrying only a 6% average refund rate — consistent
with its outsized share of total order volume. AirPods alone account for 2,636 refunds
at 49% of total refund share, making it the single largest operational refund burden
in the portfolio despite a relatively modest 5% refund rate.

- **Brand-Level Refund Risk:** Apple accounts for ~3,000 refunds at a 6% refund rate across
its full product lineup. Lenovo's single ThinkPad product sits at 12% and 343 refunds —
a disproportionately high rate for its volume. Samsung and Bose show the lowest refund rates
and counts, though Bose's 0 refunds across 4 years likely reflects its extremely low order
volume (27 orders) rather than product quality. Premium price tier products carry the
highest refund rate overall at 7% across ~4K refunds.

<div align="center">
  <img src="images/refund_by_product_year.png" width="75%">
</div>

- **Lenovo Carries the Highest Risk by Rate:** While Apple dominates by volume, Lenovo's
ThinkPad carries the highest refund rate in the portfolio at 12% with
MacBook Air close behind at 11%. At AOVs of $1,100 and $1,588
respectively, each return from these products carries significant financial impact
relative to lower-priced items.

- **2020 Saw a Dramatic Refund Spike Across All Products:** AirPods alone generated
~1,550 refunds in 2020 — nearly double their 2019 volume — consistent with the
pandemic-driven order surge. Gaming Monitor followed with ~800 refunds. All products
normalized sharply in 2021 before the 2022 data gap emerged.

- **Data Integrity Flag — 2022 Refunds:** Refund data appears incomplete for 2022. With
21,565 orders placed that year, a refund rate consistent with prior years would suggest
approximately 1,000+ refunds — yet 2022 shows no refund records in the dataset. Definitive
conclusions on refund trends should be treated with caution until 2022 data is fully
validated.

- **Loyalty vs. Non-Loyalty Refund Behavior:** Loyalty members are refunding more than
non-loyalty customers (2.8K vs. 2.5K) despite placing fewer total orders. In 2020 both
groups peaked at 1.6K and 1.4K respectively, but 2021 saw non-loyalty refunds drop sharply
to 288 while loyalty remained elevated at ~1K. Notably, loyalty members' average refund
value is significantly lower at $297 vs. $549 for non-loyalty — suggesting loyalty members
return lower-value items more frequently.

*When refund behavior is segmented by loyalty status, a more specific pattern emerges —
one that raises broader questions about the effectiveness of TechHaven's loyalty program
overall. See [Loyalty Program Performance](#loyalty-program-performance) below.*

## <ins>Loyalty Program Performance<ins>
*Despite a lower Average Order Value, loyalty members have demonstrated greater revenue 
stability and resilience during downturns — making a strong case for continued investment 
in the program.*

![Loyalty Program Chart](images/loyalty_performance.png)
*Despite early promise, the loyalty program shows structural weaknesses —
near-zero repeat purchase rate, higher refund frequency, and eroding AOV advantage
point to a program in need of significant restructuring.*

<div align="center">
  <img src="images/loyalty_sales_aov.png" width="45%">
  <img src="images/loyalty_refunds.png" width="45%">
</div>

- **Revenue Contribution:** Since Q2-2021, loyalty members have generated higher 
total sales compared to non-loyalty customers. Totalling $10M between 2019-2022.

- **Retention Rate:** Of 45,693 loyalty members, only 39 made more than 1 purchase on
i different date - a repeat purchase rate of essentially 0% and sales of $29K. For a program designed
to drive retention and repeat buying behavior, this is a significat failure signal.
The program is enrolling members but not changing their purchasing behavior.

- **AOV Uptick Temporary:** Loyalty members generally carry a lower AOV than non-loyalty customers, 
though the gap narrowed in 2022 as non-loyalty AOV declined while loyalty AOV remained 
stable. This was not because loyalty members spend more, as AOV remained flat. Non-Loyalty AOV spiked
during the pandemic then sharply declined back to loyalty levels by 2022, overtaking loyalty by Q4-22.
This stability suggests loyalty members are less sensitive to the broader market 
conditions that drove non-loyalty customers to spend less per order. Not loyalty strength.

- **Non-Loyalty Pulling Ahead in Q4 2022:** By Q4 2022 non-loyalty has overtaken
loyalty on both total sales and AOV — erasing what appeared to be the program's key
advantages. With both metrics now converging or reversing, the data no longer supports
the narrative that loyalty members are more valuable customers.

- **Loyalty Members Refund More Despite Fewer Orders:** Loyalty members generate more
refunds than non-loyalty customers despite placing fewer total orders (45K vs. 62K), and tend to
return lower-value items. This points to more lenient return expectations among loyalty members
and warrants monitoring to avoid policy abuse.

- **Non-Loyalty Refunds Carry Higher Financial Impact:** Despite loyalty members
refunding more frequently, non-loyalty refund AOV spiked to ~$400 in 2020 vs.
loyalty's stable ~$200. By 2022 both have converged around $220–$230.

<div align="center">
  <img src="images/loyalty_decomp_sales.png" width="45%">
  <img src="images/loyalty_decomp_orders.png" width="45%">
</div>


- **Program Verdict — Restructure Required:** The loyalty program is not delivering
on its core premise of retention and repeat purchase behavior. With a 0% repeat purchase rate, higher
refund frequency, and declining performance advantages by end of 2022, the program requires
significant restructuring.

### <ins>Marketing Channel Performance<ins>
*The Direct channel dominates TechHaven's order volume by a wide margin, while the Affiliate 
channel punches above its weight on order value — pointing to an underinvested but 
high-potential acquisition channel.*

![Marketing Channel Chart](images/marketing_channel.png)
*Email is the standout marketing channel — the only one to show growth in both 2020
and 2021 — and serves as the primary touchpoint for loyalty members. While Direct
traffic dominates overall revenue, it reflects organic behavior rather than managed
marketing activity.

- **Direct Traffic Dominates Revenue but Reflects Organic Behavior:** Direct
accounts for $23M (~82%) of total revenue and was the primary driver of the 2020
pandemic spike. As an organic channel rather than a managed one, its dominance
reflects strong brand awareness.

- **Email is the Only Channel to Grow in Both 2020 and 2021:** While every other
channel declined in 2021 after the pandemic spike, Email continued to grow -
+222.60% in 2020 followed by +24.46% in 2021. This makes Email the only one
that sustained momentum beyond the pandemic period.

- **Affiliate Channel Opportunity:** Despite its low order volume, Affiliate delivers the 
highest AOV of any channel at ~$303 — suggesting it consistently attracts higher-intent, 
higher-value customers. This channel appears underinvested relative to the quality of 
customers it brings in.

- **Unknown Channel Anomaly:** The Unknown channel spiked +2,325% in 2020 and +295% in 2022 - sharply contrasting with declines across all other channels in the same periods. This is almost certainly a tracking or attribution issue and should be investigated and resolved before drawing any conclusions from this channel's performance.



### <ins>Regional Performance<ins>
*TechHaven's performance is heavily concentrated in North America and EMEA, though growth 
and decline patterns are broadly consistent across all regions — with LATAM emerging as a 
notable exception with its own distinct seasonality.*

<div align="center">
  <img src="images/regional_brand.png" width="45%">
  <img src="images/sales_region.png" width="45%">
</div>

- **Regional Sales Concentration:** North America is the clear leader, accounting for ~54% 
of total revenue ($14M), followed by EMEA at ~30% ($8M). The remaining regions make up a 
relatively small share of total sales, highlighting both how dependent TechHaven is on these 
two markets and the untapped growth potential elsewhere.

- **Consistent Growth & Decline Patterns:** Growth and decline trends were largely mirrored 
across all regions throughout 2019–2022 — the 2020 pandemic spike, 2021 peak, and 2022 
contraction were global in nature. However, North America deviated slightly, experiencing a 
smaller decline in 2021 (-16%) compared to other regions, before seeing a relatively steeper 
drop in 2022 (-39%).

- **Holiday Seasonality Across Regions:** November and December represented peak growth 
periods across NA, EMEA, and APAC, consistent with holiday-driven demand patterns. This 
alignment suggests a shared customer behavior across these markets that can be planned 
around with coordinated seasonal campaigns.

- **LATAM Seasonality Divergence:** LATAM stands out as the only region that deviates from 
the broader holiday seasonality pattern, showing its strongest performance in July rather 
than November–December. This suggests region-specific demand drivers that warrant a tailored 
marketing approach rather than a one-size-fits-all global campaign strategy.
