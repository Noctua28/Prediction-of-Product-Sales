<p align = "center"> 
  <img src = "Data Science cover.png">
</p>

# Prediction-of-Product-Sales
## Predicting the sales of various objects.

**Author**: 
Aharon Brenes 

### Business problem:

There is a need for sales predictions to help businesses optimize their inventory management, pricing strategy, and overall revenue. The dataset used includes features such as product type, price, and promotion status, as well as external factors like holidays and economic indicators.The goal was to build a model that accurately predicts sales and provides insights to improves sales performance and make data-driven decisions to optimize their operations.


### Data Source:
[Big Mart Sales Prediction from Analytics Vidhya](url)


## Data Dictionary

<p align = "center"> 
  <img src = "Data Dictionary.png">
</p>



## Model

### Linear Regression

Our Linear Regression model identified several impactful features.

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/84cd5ab3-e5c1-4a28-a5c5-cebb3051183f)

Here are interpretations of the top 3 most impactful features:

1. Item_MRP: This feature represents the Maximum Retail Price (MRP) of the item. If the coefficient for this feature is positive, it means that items with a higher MRP are likely to have higher sales, assuming all other features remain constant. On the other hand, if the coefficient is negative, it would suggest that as the MRP of an item increases, the sales for that item are likely to decrease, assuming all other factors remain constant.



2. Outlet_Type_Supermarket Type3: This feature is a result of one-hot encoding of the Outlet_Type category. A positive coefficient for this feature would mean that items sold in "Supermarket Type3" outlets tend to have higher sales compared to other types of outlets, assuming all other factors remain constant. A negative coefficient would suggest the opposite.



3. Item_Visibility: This feature represents the percentage of total display area of all products in a store allocated to the particular product. A negative coefficient for this feature would mean that as the visibility of an item increases (i.e., it occupies a larger percentage of the display area), the sales for that item tend to decrease, assuming all other factors remain constant. This could be due to the product being too common or not having enough appeal. A positive coefficient would suggest that higher visibility leads to higher sales, as the product is more noticeable to customers.

### Random Forest

Our Random Forest model provided an analysis of feature importances.

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/6632637f-9839-483f-8a46-0c33fdd05b91)


Here are interpretations of the top 5 most important features:

1. Item_MRP: Similar to the interpretation in the Linear Regression Model, this feature's importance in the Random Forest Model suggests that the MRP of an item plays a significant role in predicting the sales of the item.



2. Outlet_Type_Supermarket Type3: Similar to the interpretation in the Linear Regression Model, the importance of this feature in the Random Forest Model suggests that the type of outlet in which an item is sold significantly influences the sales of the item.



3. Item_Weight: The importance of this feature suggests that the weight of the item significantly influences its sales. This could be because heavier items might be bulk goods or premium products, which could either increase or decrease sales depending on the context.



4. Outlet_Establishment_Year: The importance of this feature suggests that the year the outlet was established plays a significant role in predicting sales. Older outlets may have a loyal customer base leading to higher sales, or they might have lower sales due to being outdated.



5. Item_Visibility: Similar to the interpretation in the Linear Regression Model, the importance of this feature in the Random Forest Model suggests that the visibility of an item in a store significantly influences the sales of the item.

## Bar Plot

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/ffa6099a-8a0d-4a58-8991-f7653ca2e439)

This plot represents the average impact of each feature on the model's output. The y-axis shows the names of the features, and the x-axis represents the average absolute SHAP value, a measure of the magnitude of a feature's effect on the output. The larger the SHAP value, the higher the impact of the feature on the model's prediction.

The SHAP values and Random Forest's feature importance don't completely align, and here's why:

1. SHAP values take into account not only the direct impact of a feature on the output but also its interaction with other features. This makes SHAP values a more comprehensive measure of feature importance.


2. The Random Forest model rates Item_MRP as the most important feature, while SHAP values rank Outlet_Type_Supermarket Type3 at the top. This could be because traditional feature importance measures like those from a Random Forest may be biased towards variables that have more categories or are numeric.


## Dot Plot

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/5c38ac2f-7158-436c-96c8-037284b0a952)

This plot shows the impact of each feature on the model's prediction for individual instances. Each dot represents an instance (or a row) from the dataset. The color represents the feature's value (high in red, low in blue). The position on the x-axis shows whether the effect of that value is associated with a higher or lower prediction.

1. Outlet_Type_Supermarket Type3: This feature has the most significant impact on sales. If a store is a "Supermarket Type3", it tends to be associated with higher sales. Conversely, if a store is not of this type, it is likely to have lower sales.

2. Item_MRP: This is the price of the product. More expensive items (Item_MRP high, shown in red) are associated with higher sales, while cheaper items (low Item_MRP, shown in blue) tend to have lower sales.

3. Outlet_Type_Grocery Store: If an outlet is a grocery store, it is likely to have lower sales. If it's not a grocery store, the sales are likely to be higher.

### For further information
For any additional questions, please contact aharon.brenes@gmail.com
