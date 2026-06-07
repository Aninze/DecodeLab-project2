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

![Alt text](https://github.com/Aninze/DecodeLab-project2/blob/main/Totalprice%20outlier%20detection.png?raw=true)
