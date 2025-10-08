# Project Background
<p align="center">
  <img src="WebOne Gadgets Logo - Tech-Savvy Aesthetic.png" alt="WebOne Gadgets Logo" width="256" height="256">
</p>

WebOne Gadgets is a global online e-commerce platform selling popular consumer electronics from brands like Apple, Samsung, and Lenovo since late 2018 through its website and mobile app. Its main marketing channels are SEO, email, social media, and affiliate, and it measures performance using Revenue, Order Count, and Average Order Value (AOV). Together with the Head of Operations, this analysis examines sales transactions from 2019-2022 and compares metrics across Sales Trends, Seasonality, Loyalty Program Performance, and Refund Rates.

Business questions answered through SQL queries: [link] | ERD: [link]

# Executive Summary

### Overview of Findings

North Star Metrics: **$28M Revenue | 108k Order Count | $260 AOV**

<p align="center">
  <img src="Sales Trends - Revenue & AOV.png" alt="Sales Trends - Revenue & AOV" width="50%">
</p>

- Revenue grew steadily on launch and reached a record $10.1M in 2020, driven by pandemic spending on laptops and gaming monitors from non-loyalty customers. Following this peak, laptop prices gradually dropped and customers started to order less, leading to a sharp fall across all metrics which culminated in an unusually poor Q4-2022.
- Loyalty program members brought in 39% of Revenue across all 4 years which increases to 54% between 2021-2022. Meanwhile, 42% of non-members' $17.1M Revenue comes from 2020 alone, suggesting one-off, pandemic-driven purchases. Additionally, member AOV remained consistent around $250 from 2021 through Q3-2022, while non-member AOV dipped from $375 in Q4-2020 to $213 in Q3-2022.
- Overall Refund Rate: ~7.8%. Customers sought refunds at higher rates for pricier products like laptops (16%) & gaming monitor (9.5%). Loyalty members sought double the refunds (11.4%) as non-members (5.8%), particularly for Airpods & gaming monitor.

### Recommendations

Based on the above findings, we recommend the following:
- Revise 2023-2024 Revenue forecasts to pre-pandemic baseline levels and focus on sustained growth in subsequent years, for the Finance Team.
- Optimise product portfolio to focus on 4 main products, add complimentary branded accessories, and expand into mid-range price tiers, for the Product & Sales Teams.
- Strengthen loyalty program by adding preferred products, premium pricing tiers, and sending satisfaction surveys, for the Marketing Team.
- Work with suppliers to address quality control issues, negotiate acceptable refund levels & appropriate penalties, and revise company's refund policy by charging restocking fee for non-defective refunds, for the Operations & Finance Teams.

# Insights Deep Dive
### Sales Trends:

<table align="center" width="100%">
  <tr>
    <td><img src="Product Revenues.png" alt="Area chart showing revenues per product" width="100%"></td>
    <td><img src="Marketing Channels.png" alt="Area chart showing revenues per marketing channel" width="100%"></td>
  </tr>
</table>

* **4 Products make up 96% of Revenue:** 27" 4K Gaming Monitor, Apple Airpods (most popular - 48k Order Count), two laptops (Apple Macbook Air, Lenovo ThinkPad). Laptop Revenue doubled to $1.3M in Q4-2020 from $0.54M in Q4-2019, and then fell 90% to $0.13M in Q4-2022. Apple products made up 52% of Revenue in 2020-2021, which fell to 41% in Q4-2022. WebOne's core products are in clear decline which make it critical to immediately conduct competitor pricing analysis. The Product Team can look into introducing mid-tier laptops to capture demand from price sensitive segments.
  
* **Direct marketing brings in 83% of Revenue:** SEO performs well and brings in a higher AOV ($277) than email ($180). Order placed on the web page further contribute 97% of Revenue, and mobile orders contribute the remaining 3%, signalling underperforming mobile channels that represent wasted marketing expenditure. The Marketing Team could audit the mobile app's user experience & ROI, eliminating it entirely if required.
  
* **12 countries make up 80% of Revenue.** WebOne's global reach to 192 countries is concentrated in a handful of key markets: US (47% of Revenue), UK, Canada, Japan, Germany, Australia, Brazil, France, Spain, Netherlands, Italy, and India. AOV in the APAC region is the highest ($278), followed by North America ($260), EMEA ($258), and LATAM ($231), signalling price sensitivity and varying product preferences by region. The marketing team could focus expenditure in these countries while the product & sales team could look into creating region-specific bundles based on AOV.


### Seasonality & Growth Rates:

<table align="center" width="100%">
  <tr>
    <td><img src="Monthly Growth Rates.png" alt="Monthly Growth Rates" width="100%"></td>
    <td><img src="Quarterly Regional Revenue Growth.png" alt="Quarterly Regional Revenue Growth" width="100%"></td>
  </tr>
</table>

* **Pandemic spending spike was an anomaly.** Consistent monthly growth from March to August 2020 suggests exceptionally high demand for electronics during the pandemic. Yearly growth rates (2019-2020): 100% Order Count | 160% Revenue | 30% AOV; suggest that company growth was anchored to 2020 and a subsequent return to normalcy in 2022 to pre-pandemic levels. The Finance Team could look into appropriately revising 2023-2024 forecasts based on 2019 levels.

* **Seasonality and anomalously poor Q4-2022:** Best-performing months were November & December, and September for more premium products from 2019-2021. Worst months were consistently February and October. These patterns did not carry through to 2022: September was flat and October had a sharper dip of -55% (Revenue) which made Q4-2022 the company's worst performing quarter. The company should investigate contributing factors behind this decline in further detail.

* **Consistent regional trends with differences in magnitude.** Evidenced by similar quarterly percent changes in Revenue, all 4 regions experience similar overall trends. Comparing Revenues across regions highlights differences in spending patterns: EMEA drove a strong Q4-2020 with 27% increase in Revenue. LATAM grew 18% in Revenue across Q2 & Q3-2022. Targeted marketing efforts through localised campaigns could lead to capitalising on region-specific differences.


### Loyalty Program Performance:

<p align="center">
  <img src="Loyalty Rev_AOV.png" alt="Loyalty Revenue and AOV" width="50%">
</p>

* **Diverging loyalty & non-loyalty sales trends:** Loyalty members made up 54% of Revenue in 2021-2022 with non-loyalty members driving pandemic spending in 2020, highlighting long-term value of the loyalty program to the company. Calculating Customer Lifetime Value (CLV) and understanding this segment's needs could lead to further improvements in the loyalty program to drive Revenue & AOV growth.

<p align="center">
  <img src="Loyalty Channels.png" alt="Loyalty Marketing Channels" width="50%">
</p>

* **Email and direct marketing lucrative for loyalty members:** Marketing channel performance diverges over time for members & non-members. From 2019-2020 levels, direct marketing Revenue to non-members declined by $3.5M and increased by $3M to members. Email marketing AOV from members ($228) is twice as high as non-members ($105), and Revenue performance has significantly diverged. The Marketing Team may reallocate non-member email marketing spend to member retention programs.

<p align="center">
  <img src="Loyalty Products.png" alt="Loyalty Product Performance" width="50%">
</p>

* **Accessories preferred by loyalty program members:** Airpods & Webcam are more popular among loyalty members. They also pay more on average for Airpods, Gaming Monitor, & Macbook. This may be due to non-members receiving deep discounts to encourage purchases, which requires further analysis. Meanwhile, the Product & Sales Teams may consider expanding accessories to brand-specific cases, keyboards, etc., and creating product + accessory bundles targeted to loyalty members. They may also consider creating premium membership tiers with access for specific premium products reserved to high-spending loyalty customers.

### Refund Rates:

<p align="center">
  <img src="Product Refund Rates.png" alt="Product Refund Rates" width="50%">
</p>

* **High refund rates cause important lost revenues.** Overall Refund Rate (7.6%-8%) is skewed towards pricier products: laptops (16% - just under 1 in 6), Gaming Monitor (9.7%), iPhone (11%). Since this leads to high levels of lost revenues, the Operations Team could implement quality control checks on main products and negotiate guarantees with suppliers to reduce the overall refund rates.

<p align="center">
  <img src="Loyalty Refund Rates.png" alt="Loyalty Refund Rates" width="35%">
</p>

* **Loyalty program members seek more refunds.** Loyalty members seek almost double (11.4%) the number of refunds as non-members (5.8%). There are no significant differences in delivery times between loyalty and non-loyalty customers. The Sales Team could implement post-purchase check-in calls with customers to detect issues early, and the Marketing Team could implement 10% restocking fees on members if products are not found to be defective.

<p align="center">
  <img src="Loyalty_Products Refund Rate Table.png" alt="Loyalty Products Refund Rate Table" width="50%">
</p>

* **Different problem products for loyalty members and non-members:** As highlighted in the table above, loyalty members & non-members have different 'problem products', and these are skewed towards high AOV products. The sales pipeline from supplier to group-wise refunds requires deeper analysis to spot patterns and take appropriate preventive action to reduce lost revenue in the future.


# Recommendations:

Based on the insights and findings above, we recommend the following: 

* **Set Revenue Forecasts using Pre-Pandemic Baseline:** Revenue peaked in 2020 ($10.1M), 42% of loyalty non-member Revenue came from 2020 alone, and Q4-2022 was the worst quarter since inception. WebOne Gadgets has, so far, relied on one-time pandemic spikes to grow, and its current declining Revenue trajectory poses a threat to profitablity. Therefore, we recommend that the Finance Team revise 2023-2024 Revenue forecasts to stabilise Revenue to a pre-pandemic baseline and then focus on sustained growth for the following years.

* **Optimise Product Portfolio:** The 4 core products that make up 96% of Revenue have shrunk since 2020. The Product Team should immediately conduct competitor pricing benchmarks. We recommend the Product & Sales Teams to eliminate products outside these core products, introduce complimentary accessories (keyboards, branded cases, chargers, headphones), and expand into a mid-price tier to capture demand from price sensitive segments.
  
* **Focus on High-Value Markets:** 12 countries account for 80% of Revenue and regional differences in AOV represent untapped market opportunities. We therefore recommend the Marketing Team to introduce market-specific campaigns in these countries geared towards specific pricing tiers (eg., APAC - Premium), to boost market penetration in these countries and regions.
  
* **Leverage Seasonal Patterns:** Orders consistently peaked during September, November, and December. We recommend the Sales & Product Teams to create back-to-school & holiday product bundles, and the Marketing Team to boost early marketing efforts towards the end of August & October to capitalise on increased seasonal demand. We recommend the Operations Team to appropriately stock up on inventory to ensure timely delivery and customer satisfaction during peak months.
  
* **Strengthen Loyalty Program:** Loyalty program members made up 54% of Revenue in 2021-2022 with a higher AOV during this time than non-members. Owing to strong long-term performance, recommend the Marketing Team to further strengthen the loyalty program. Besides adding accessories that loyalty members prefer, we recommend reallocating marketing resources to focus on customer retention and calculating a CLV metric to estimate the overall value of retaining a customer for the company. We also recommend the Marketing Team to launch a targeted survey to better understand & respond to the needs of this segment.
  
* **Address Quality Control Issues & Refund Policy:** Laptop refund rates were 16% and overall refund rates 7.6%-8%. Lost revenue was higher because pricier products have higher refund rates, signalling issues in quality control and refund policy. We therefore recommend the Operations Team to implement quality control checks on inventory purchase for top products and negotiate acceptable baselines & appropriate penalties with suppliers. We also recommend the Finance & Marketing Teams to revise refund policy and implement restocking fees in case of non-defective products.


# Assumptions and Caveats:

Throughout the analysis, multiple assumptions were made to manage challenges with the data:

* No recorded refunds after 14/07/2021 & refund timestamps recorded 2 years after purchase timestamps. Data until this point (69k orders) was used to estimate true refund rates.
  
* Joining all 4 tables together caused 169 orders (0.16%) to be duplicated. These were included in the analysis.

These require further investigation with the data engineering team to address the underlying data collection & validation issues.