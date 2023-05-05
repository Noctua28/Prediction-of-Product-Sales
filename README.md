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

## Methods
Data exploration and visualization

Data preprocessing techniques including handling missing values and categorical features, and scaling/normalization

Linear regression modeling to predict sales

Decision tree modeling to predict sales

Random forest modeling to predict sales

Model evaluation using R^2 and RMSE metrics.

## Results

#### Sales by Location Type
<p align = "center"> 
  <img src = "Sales by Product Type.png">
</p>



**Location Type:** The location of the store plays an important role in the sales of products. In our dataset, we found that products sold at stores located in Tier 1 cities have higher sales compared to products sold at stores located in Tier 2 and Tier 3 cities.

#### Sales by Item Type

<p align = "center"> 
  <img src = "Location type.png">
</p>



**Item Type:** The type of product also has a significant impact on its sales. In our dataset, we found that certain types of products such as "Health and Hygiene" and "Household" have higher sales compared to other types of products.

## Model

We built and evaluated two machine learning models for this project: a linear regression model and a regression tree model. The performance of each model is summarized below:

Linear Regression Model:
R^2: 0.578
RMSE: 1071.20

Regression Tree Model:
R^2: 0.193
RMSE: 1480.81

Based on the evaluation metrics, we recommend using the linear regression model to predict the sales of products at Big Mart. The linear regression model had a higher R^2 value and a lower RMSE value, indicating that it is a better fit for this dataset.

## Recommendations:

Based on the analysis of the data, it is evident that the location and item types significantly impact the sales of products at Big Mart. My analysis reveals that promoting high-selling products in their respective locations and stocking them adequately is crucial in optimizing inventory management. Additionally, we recommend analyzing sales of different product types and adjusting inventory accordingly to maximize sales. Collecting data on sales and implementing the recommended model will enhance our sales forecasting accuracy and improve inventory management and supply chain operations. This will help us anticipate demand better, ensuring we have the right products in the right stores at the right time. By doing so, we can reduce costs related to overstocking and understocking while increasing revenue from improved customer satisfaction and loyalty.


## Limitations & Next Steps

Limitations:

The data set only includes information from 10 stores, which may not be representative of all Big Mart stores.
The data set does not include information about promotions, events, or other factors that may impact sales.
The data set only includes information from a single year, which may not be representative of sales patterns over a longer period of time.
The data set contains missing values that were imputed using the most frequent value, which may not be the most accurate way to fill in missing values.

Next steps:

Collect and analyze data on promotions, events, and other factors that may impact sales to better understand their impact on sales.
Gather data from additional stores to ensure that findings are representative of all Big Mart stores.
Collect and analyze sales data over a longer period of time to identify sales patterns and trends over time.
Explore alternative methods for imputing missing values, such as using a predictive model or filling in missing values based on patterns in the data.


### For further information
For any additional questions, please contact aharon.brenes@gmail.com
