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

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/63af4af2-fda9-436e-a905-f5133e63eb17)

Here are interpretations of the top 3 most impactful features:

1. Outlet_Type_Grocery Store (Coefficient: -1726.6760):

Interpretation: For every unit increase in the presence of a grocery store outlet type (i.e., if an item is sold in a grocery store), the predicted sales decrease by approximately 1726.68 units of currency. This suggests that selling an item in a grocery store is associated with lower sales compared to other outlet types.

2. Outlet_Type_Supermarket Type3 (Coefficient: 1610.5642):

Interpretation: For every unit increase in the presence of a Supermarket Type3 outlet (i.e., if an item is sold in a Supermarket Type3), the predicted sales increase by approximately 1610.56 units of currency. This indicates that selling an item in a Supermarket Type3 is associated with higher sales compared to other outlet types.

3. Item_Visibility (Coefficient: -464.6734):

Interpretation: For every unit increase in item visibility (measured as the percentage of display area allocated to the item in a store), the predicted sales decrease by approximately 464.67 units of currency. This may seem counterintuitive, as we might expect higher visibility to lead to higher sales. However, this negative coefficient could be capturing other factors or relationships in the data, such as discounts on highly visible items leading to lower overall revenue. It would be valuable to investigate this relationship further.

### Random Forest

Our Random Forest model provided an analysis of feature importances.

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/80d8ed07-3203-44ef-b5d0-4c4db260d9d0)

Here are interpretations of the top 5 most important features:

1. Item_MRP (Maximum Retail Price):
   
Interpretation: The maximum retail price of an item is a crucial factor in determining its sales. Higher-priced items may generate more revenue, while lower-priced items may appeal to budget-conscious customers. The importance of this feature suggests that pricing strategies can significantly influence product sales.

2.Outlet_Type_Grocery Store:

Interpretation: The type of outlet, specifically whether it is a grocery store, plays a significant role in sales. Items sold in grocery stores may experience different sales patterns compared to other outlet types. This could be due to the types of products typically found in grocery stores or the shopping behavior of customers in these stores.

3.Item_Visibility:

Interpretation: How visible an item is within the store affects its sales. Highly visible items may catch customers' attention more easily, but as noted in the linear regression interpretation, there may be complex factors at play. Understanding how to optimize product placement and visibility could enhance sales performance.

4. Outlet_Type_Supermarket Type3:

Interpretation: Similar to the grocery store outlet type, the presence of a Supermarket Type3 outlet influences sales. This outlet type may offer a different shopping experience, product selection, or pricing structure that attracts a specific customer base. Understanding the characteristics of different supermarket types can help in tailoring marketing and sales strategies.

5. Item_Weight:

Interpretation: The weight of an item is also identified as an important feature. The weight may be indicative of the product's size, quantity, or quality, all of which could influence consumer purchasing decisions. Heavier items might be associated with bulk products or higher quality, while lighter items might be more convenient for certain customers.

For more information contact Aharon Brenes (aharon.brenes@gmail.com)
