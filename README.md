# Segment the customers of an e-commerce site

"A good level of customer knowledge allows the company to better know those who contribute to its commercial prosperity, in particular information on their profiles, their needs, their centers of interest and their expectations."

During this this project I will use the KMeans Clustering technique to provide actionable customer segments to an e-commerce site. Then I will proceed to the evaluation of the maintenance frequency based on an analysis of the stability of the segments over time. 

# Table of contents

1. [Problem description](#problem-description)
2. [Data cleaning](#data-cleaning)
3. [Data analysis overview](#data-analysis-overview)
4. [Modelization](#modelization)
5. [Results](#results)
8. [Business interpretation overview](#business-interpretation-overview)

# Problem description

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_desc.png" width="1200">

[Back to table of contents](#table-of-contents)

# Data cleaning

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_data_cleaning.png" width="600">

[Back to table of contents](#table-of-contents)

# Data analysis overview

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_recency.png" width="600">

1. Sales order recency has an empirical distribution ranging from 0 to 695 days
2. On average, a customer placed their last order 238 days ago
3. Half of the orders are less than 220 days old and 75% less than 347 days old

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_amount.png" width="600">

1. The average basket has a value of 212.07 reals
2. The median is 113.01 reals
3. 75% of orders have a value of less than 201.98 reals

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_correlation.png" width="600">

1. The total_orders and total_products variables, with a correlation coefficient of 0.646 and a p-value of 0, are probably dependent (p-value < 0.05)
2. Similarly, with a correlation coefficient of 0.486 and a p-value of 0, the variables total_payment_installations and total_products are probably dependent
3. The other variables are either weakly correlated or independent


[Back to table of contents](#table-of-contents)

# Modelization

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_model.png" width="1200">

[Back to table of contents](#table-of-contents)

# Results

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_results.png" width="600">

To select the best combination, I classify each of the scores from the best to the worst and I award 5 points to the best, then 4 to the next etc… then finally 0 to the worst

[Back to table of contents](#table-of-contents)

# Business interpretation overview

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_silhouette.png" width="600">

<img src="https://raw.githubusercontent.com/jamesbarthelemy/images/main/p4_cluster.png" width="600">

1. With 28893 clients, or 31.15% of the total clients of olist, cluster 0 is the second largest cluster
2. It groups together customers who have ordered rather recently for an average number of orders and products ordered
3. The average basket is the second weakest
4. It represents the second group of most satisfied customers

[Back to table of contents](#table-of-contents)
