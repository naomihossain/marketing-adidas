# marketing-adidas
Researching sales on Adidas

# Objective 
What is the impact of sales channel, region, and product category on Adidas operating profit?

Our goal was to determine whether product attributes, regional differences, or other market characteristics have a significant impact on sales outcomes. By closely evaluating Adidas’s performance across regions and product categories, we aim to provide data-driven insights and recommendations that can help the company enhance its competitive position and overall success.

# Dataset
This dataset was found on Kaggle and was  publicly posted as ‘Adidas Sales Dataset’. Since this data is available to the public our group did not have to collect this dataset through methods such as surveys, scraping, or internal company systems. There is limited information on the raw data-collection of this dataset. The dataset provides detailed transactional information capturing sales activity across various retailers, product categories, and regions in the United States. The data was sourced from a Kaggle dataset that contains 9,648 records of Adidas purchases with 13 variables. The data focuses on U.S. regional sales from 2020 to 2021.

# Exploratory Data Analysis
In-store profit dominates the other two sales channel. It is followed by Outlet then Online. 
<knb><img width="535" alt="image 1" src="images/image 1.png"></kmb>

The Southeast region has the highest profit compared to all the other regions. The Midwest and Northeast are weaker.
<knb><img width="535" alt="image 2" src="images/image 2.png"></kmb>

The product with the most profit is men’s street footwear. This is what adidas has always been known for. 
<knb><img width="535" alt="image 3" src="images/image 3.png"></kmb>

Form the heatmap:
* it shows average operating profit across the five regions.
* The most profitable combination is Southeast region in-store purchases with the highest average profit at 131,869.
* The lowest profitable combination is Northeast online sales with only 2,400.
<knb><img width="535" alt="image 4" src="images/image 4.png"></kmb>

# Regression Analysis
The regression model is statistically significant (p < 0.001).
Sales Channel: In-store sales deliver the highest profitability; Online and Outlet underperform.
Region: The Southeast region yields the highest profit; the Northeast and West show weaker performance.
Product: Men’s Street and Athletic Footwear are the strongest profit drivers.
Price Effect: Higher price per unit increases operating profit.
Although our R² is 0.34, which
* is moderate, the model is statistically significant where (F = 419.9 p <0.001). Therefore, this shows our model is valid and strong.

<knb><img width="535" alt="image 5" src="images/image 5.png"></kmb>
<knb><img width="535" alt="image 6" src="images/image 6.png"></kmb>

# Interaction Analysis
Testing the relationship between Sales Channel and Operating Profit varies across regions or products.

In this model, the baseline categories are: 
Sales Method - in store
Region - Midwest
Products - Men’s Apparel

<knb><img width="535" alt="image 7" src="images/image 7.png"></kmb>

This table shows the interaction effect of Sales Channel and Region:
* Significant interaction effects exist between Sales Method and Region (R² ↑ from 0.34 → 0.37).
* Online and Outlet channels perform significantly worse in Southeast, West, and Northeast regions compared to the baseline.
* No significant interaction found in the South region, suggesting stable channel performance there.
* Managerial Implication: Regional strategy adjustments are needed  strengthen In-store presence and improve Online/Outlet logistics or promotions in weaker regions.

<knb><img width="535" alt="image 8" src="images/image 8.png"></kmb>




