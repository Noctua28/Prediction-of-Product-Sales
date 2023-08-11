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

### Explaining our tree-based model with SHAP

****![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/3a23fae5-8865-4f27-a157-183ba63cf416)

The bar summary plot shows the average magnitude of the SHAP values for each feature, providing a global view of feature importance. The y-axis shows the names of the features, and the x-axis represents the average absolute SHAP value, a measure of the magnitude of a feature's effect on the output. The larger the SHAP value, the higher the impact of the feature on the model's prediction.

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/c4656aa0-4f6a-418e-a9c3-5b8648e7e8e0)

The dot summary plot shows the SHAP values for individual data points, allowing us to understand how each feature influences individual predictions.

1. Item_MRP

Item MRP (Maximum Retail Price) is the first most important feature.

In the dot summary plot, we can examine the distribution of SHAP values for this feature. If the values are mostly positive, it indicates that higher MRP generally leads to higher predicted sales. If they are tightly clustered, the influence is consistent across different data points.

2. Outlet_Type_Supermarket Type3

Outlet Type: Supermarket Type3 is the second most important feature.

Look at the spread of SHAP values for this feature in the dot summary plot. If the values are mostly positive, it may indicate that this type of supermarket has a positive influence on predicted sales. The spread of the values can indicate whether this influence is consistent or varies.

3. Outlet_Type_Grocery Store

Outlet Type: Grocery Store is the third most important feature.

Similar to the previous feature, you can interpret its influence by examining the distribution of SHAP values in the dot summary plot. A mostly negative spread may indicate that this outlet type tends to lower predicted sales.

Summary
These three features appear to have significant influence on the model's predictions:

- Item MRP: Likely has a strong and possibly consistent influence on sales predictions.
- Outlet Types: Different types of outlets (Supermarket Type3 and Grocery Store) may have distinct effects on sales predictions, reflecting the differences in shopping behavior at various types of stores.

## LIME Tabular Explanation 

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/d2958c8b-61fc-49f9-8291-5b21caa4f161)

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/9e838996-e0c9-459b-b767-50525953b83f)

1. Low Sales Example: Features with significant negative contributions, as these may be the factors leading to lower sales. Likewise, features with positive contributions might still be encouraging sales but are not enough to result in high sales.


2. High Sales Example: Features with positive contributions are likely driving the high sales in this example. Analyze how these features differ from those in the low sales example to understand what factors are most influential.

## Interpretation Individual Force Plots 

![image](https://github.com/Noctua28/Prediction-of-Product-Sales/assets/65126638/2ae02c38-fd11-4947-a9ee-7e5caa4d77be)

1. Red vs. Blue: In a SHAP force plot, red features push the prediction higher, while blue features push it lower. You can analyze the balance between red and blue to understand what's driving the prediction.


2. Low Sales Example: Look for strong blue forces that might be pulling the prediction down, leading to low sales.


3. High Sales Example: Look for strong red forces that might be pushing the prediction up, leading to high sales.


For more information contact Aharon Brenes (aharon.brenes@gmail.com)
