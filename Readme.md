AeroFit Treadmill Dataset Analysis
==================================

Overview
--------

The AeroFit Treadmill dataset contains information about customers and their treadmill purchasing behavior. The dataset aims to uncover insights about customer preferences, purchasing trends, and relationships between demographic and usage variables.

Dataset Information
-------------------

-   The dataset contains **no null values**.
-   It includes information about **three treadmill models**:
    1.  **KP281** - Entry-level treadmill priced at **$1,500**.
    2.  **KP781** - Advanced treadmill with premium features priced at **$2,500**.
    3.  **KP481** - Mid-level treadmill for runners priced at **$1,750**.
-   **Marital Status** is categorized as:
    -   **Single**
    -   **Partnered**

Exploratory Data Analysis (EDA)
-------------------------------

### Univariate & Bivariate Visual Analysis

1.  **For Continuous Variables**:
    -   **Univariate Analysis**: Distplot, Histogram, Countplot.
    -   **Bivariate Analysis**: Boxplots, Pairplots.
2.  **For Correlation**:
    -   Heatmaps to identify relationships between numerical variables.
3.  **Outliers**:
    -   Boxplots were used to identify outliers.
    -   **Findings**:
        -   Outliers in Age, Education, Fitness, and Usage are **less than 5%**, hence not treated.
        -   Income has **10% outliers**, primarily on the higher end, so categorized.
        -   Miles has **7% outliers**, also on the higher end, and categorized accordingly.

### Correlation Analysis

-   **Positive correlations**:
    -   **Age & Income**: Older individuals tend to have higher income.
    -   **Income & Miles**: Higher-income customers tend to use treadmills more.
    -   **Usage & Miles**: Higher usage corresponds to more miles covered.
-   **Random behavior**:
    -   **Age & Miles**: No clear pattern.

### Categorization of Numerical Columns

-   **Education, Usage, Fitness** converted into categorical variables to improve insights.

### Key Inferences

-   **Education Level & Purchase Trends**:
    -   High school-educated individuals are more likely to buy a treadmill.
    -   **KP281 is the most preferred treadmill among high school graduates**.
-   **Age Group Analysis**:
    -   Customers aged **20-40 years** are the primary buyers.
-   **Usage & Product Preference**:
    -   **High-usage customers prefer premium models (KP781).**
    -   **Moderate-usage customers prefer KP481.**
    -   **Low-usage customers prefer KP281/KP481.**
-   **Fitness & Product Preference**:
    -   Higher fitness scores correlate with the purchase of advanced models.

Business Insights
-----------------

### Attribute Ranges

| Feature | Details |
| --- | --- |
| **Product** | KP281, KP481, KP781 |
| **Age** | 18 - 50 years |
| **Gender** | Male, Female |
| **Education** | 8 unique values (years) |
| **Marital Status** | Single, Partnered |
| **Usage (days/week)** | 2 - 7 |
| **Fitness Score** | 1 - 5 |
| **Income** | $29,562 - $104,581 |
| **Miles Covered (per week)** | 21 - 360 miles |

### Variable Distributions

-   **Product**: Most sales are for **KP281 (44%)**, followed by **KP481 (33%)**, and **KP781 (22%)**.
-   **Fitness**: Most customers rated their fitness as **3 (54%)**.
-   **Gender**: **Male (58%)** customers are more than female (42%).
-   **Marital Status**: **Partnered customers (59%)** are more likely to buy treadmills.
-   **Usage**: **Most customers use treadmills 3 days/week (38%)**.
-   **Age**: Majority of buyers are aged **20-30 years (61%)**.
-   **Income**: Most customers belong to the **$45k-$60k income range (49%)**.

Bivariate Analysis Findings
---------------------------

### Gender vs. Product

-   **KP281 and KP481** are equally popular among males and females.
-   **KP781 is more popular among males**.

### Education vs. Product

-   Customers with **16 years of education** prefer **KP281 and KP481**.
-   Customers with **18 years of education** prefer **KP781**.

### Marital Status vs. Product

-   Partnered customers **are more likely** to purchase all treadmill models.

### Usage vs. Product

-   Customers with **KP281 and KP481 use treadmills 3 days/week**.
-   Customers with **KP781 use treadmills 4 days/week**.

### Fitness vs. Product

-   KP281 & KP481 buyers have an **average fitness score of 3**.
-   KP781 buyers have an **average fitness score of 5**.

### Age Group vs. Product

-   **20-30 years** is the dominant buying group across all models.

### Income vs. Product

-   Customers with **$45k-$60k income buy KP281 & KP481**.
-   Customers with **>$60k income buy KP781**.

Recommendations
---------------

### Customer Profile for **KP281 (Entry-Level Model)**

-   **Target Gender**: Both Male & Female.
-   **Target Education**: 16 years.
-   **Target Marital Status**: Partnered customers.
-   **Target Usage**: 3 days/week.
-   **Target Fitness Score**: 3 out of 5.
-   **Target Age**: 20-30 years.
-   **Target Income**: $45k-$60k.

### Customer Profile for **KP481 (Mid-Level Model)**

-   **Similar to KP281**, but caters to slightly more frequent treadmill users.

### Customer Profile for **KP781 (Premium Model)**

-   **Target Gender**: Male.
-   **Target Education**: 18 years.
-   **Target Marital Status**: Partnered customers.
-   **Target Usage**: 4 days/week.
-   **Target Fitness Score**: 5 out of 5.
-   **Target Age**: 20-30 years.
-   **Target Income**: >$60k.

Conclusion
----------

The analysis of the AeroFit Treadmill dataset provides critical insights into customer behavior and preferences. By understanding the relationships between demographic and treadmill usage patterns, businesses can optimize their marketing strategies and enhance product targeting to maximize sales.

* * * * *
