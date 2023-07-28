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


### For further information
For any additional questions, please contact aharon.brenes@gmail.com
