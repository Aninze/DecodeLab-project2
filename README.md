# DecodeLab-project2
#### Exploratory Data Analysis

Exploratory Data Analysis (EDA) is the process of examining and visualizing data to uncover patterns, detect anomalies, and understand relationships among variables before formal modeling.

EDA is a critical step in data analysis where data scientists investigate datasets to summarize their main characteristics, often using visual methods and statistical graphics. It helps analysts understand the structure of the data, including the number of features, data types, distributions, and relationships between variables. EDA also identifies errors, outliers, and inconsistencies that could affect subsequent analysis or modeling.

#### Project-Goal
1. Calculate basic statistics (mean,median,Count)
2. Identify trends and Outliers
3. Summarize key observations

#### Key-Skill
1. Data analysis
2. Descriptive statistics
3. Analyticsl thinking

### Project_Analysis

**Dataset dimension**
<ul>
  <li> Number of rows: 1200 </li>
  <li> Number of Columns: 14 </li>
</ul>


**Outlier Detection**
<p> inter-Quartile-Range (IQR) Method is used to detect the outlier points in the numeric columns.</p>
<ul>
  <li> The number of outiers in Quantity Column: 0</li>
  <li> The number of outliers in Unitprice Column: 0</li>
  <li> The number of outliers in ItemsIncart column: 0</li>
  <li> The number of outliers in Totalprice column: 8</li>
</ul>

![Alt text](https://github.com/Aninze/DecodeLab-project2/blob/main/Totalprice%20outlier%20detection.png?raw=true)

**Numeric Descriptive Analysis**
<ul>
  <li> Small scale shopping : Customers purchase small quantities (1–5 items) per line item, with full cart sizes never exceeding 10 items.</li>
  <li> Mid-to-high pricing : Inventory prices span evenly from low cost to high-end values, averaging around 356.41.</li>
  <li> High-value drivers : A few large transactions peak near 3,456.40, skewing the overall revenue and pulling the average order value above the typical mid-range purchase.</li>
</ul>

![Alt text](https://github.com/Aninze/DecodeLab-project2/blob/main/Numeric%20descriptive%20analysis.png?raw=true)

**Categorical Descriptive Analysis**
<ul>
  <li> Dominant Coupon : The FREESHIP coupon is highly prevalent, appearing 622 times in the dataset.</li>
  <li> Top Product : There are 7 distinct products, with Printer being the most frequently ordered item (181 times).</li>
  <li> High Order Cancellations: The most frequent order status is Cancelled (250 times), which may indicate a systemic issue with order fulfillment or customer retention.</li>
  <li> Primary Acquisition Channel: Instagram is the top referral source, generating 259 entries.</li>
</ul>

![Alt text](https://github.com/Aninze/DecodeLab-project2/blob/main/Categorical%20descriptive%20analysis.png?raw=true)

**Correlation Analysis**
<ul>
  <li>Strongest Relationship : UnitPrice and TotalPrice share the strongest positive linear correlation (r ≈ 0.72). As unit price rises, total transaction price increases significantly.</li>
  <li>Moderate to Strong Relationships : Quantity shows substantial positive correlations with both ItemsInCart (r ≈ 0.65) and TotalPrice (r ≈ 0.62).</li>
  <li>Weakest Relationship : UnitPrice and ItemsInCart have virtually zero linear relationship (r ≈ 0.0006). The price of an individual item does not impact how many total items are placed in the cart.</li>
</ul>

![Alt text](https://github.com/Aninze/DecodeLab-project2/blob/main/Correlationship%20analysis.png?raw=true)

**CouponCode Count and Revenue performance**
<ul>
  <li>Volume Leader : FREESHIP is by far the most popular option. It drove over 51% of all transactions.</li>
  <li>Revenue Driver: FREESHIP also generated the majority of sales, contributing $657,438.40 to the business.</li>
</ul>

![Alt text](https://github.com/Aninze/DecodeLab-project2/blob/main/CouponCode%20count%20and%20Revenue%20performance%20summary.png?raw=true)

**OrderStatus Count and Revenue performance**
<ul>
  <li>Highest Revenue & Volume: The Cancelled status represents both the highest volume of orders (250) and the largest share of revenue ($276,396.21).</li>
  <li>Lowest Volume: The Delivered status holds the lowest volume of orders at 231.</li>
</ul>

![Alt text](https://github.com/Aninze/DecodeLab-project2/blob/main/Orderstatus%20count%20and%20revenue%20performance%20summary.png?raw=true)

**Payment Method Count and Revenue performance**
<ul>
  <li> Volume Leader: Online is your most frequently used channel with 258 transactions, generating the second-highest overall revenue.</li>
  <li>Value Leader: While Credit Card doesn't have the highest volume, it brings in the most overall revenue ($263,847.63) and has the highest average cart size per transaction.</li>
  <li>Underperformer: Debit Card lags behind in both total usage metrics and average ticket size compared to all other options.</li>
</ul>

![Alt text](https://github.com/Aninze/DecodeLab-project2/blob/main/Payment%20method%20count%20and%20revenue%20performance%20summary.png?raw=true)


