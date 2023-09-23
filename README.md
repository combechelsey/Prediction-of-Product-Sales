# Prediction-of-Product-Sales
## Predicting Trends of Item Sales Across an Array of Grocery Outlets

**Chelsey Combe**: 

### Business problem:

Utilizing Regression Modeling to Predict Item Sales and Uncover the Key Drivers of Success for Grocery Stores and Supermarkets!


### Data:

![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/13915534-615b-4c29-81f9-329c9cb9c6ee)

print()
print()
print()

## Methods
- Conducted data inspection and cleansing procedures, including the removal of duplicate records, standardization of value counts, outlier exploration, and meticulous data type assignment.

 -Developed comprehensive univariate and multivariate visualizations to gain deeper insights into the underlying trends and patterns within the dataset.

- Skillfully preprocessed the data to ensure its suitability for advanced machine learning modeling.

- Employed a range of sophisticated regression modeling techniques to extract valuable regression metrics and uncover correlations among key features.  

print()
print()

## Results

#### Classification of Items Inclued in Analysis 
![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/1ffb9905-dae4-472b-9c42-bf7ad4297583)


#### Outlet Sales by Item Type
![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/03872d47-815e-462b-9a16-c858d51e3640)


#### Total Item Sales by Outlet Size
![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/0f38ad9b-841b-4d06-a992-ae338b3d483e)

#### Total Item Sales by Outlet Type
![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/f5088429-5a28-443b-ad32-df30cf46284b)


print()
print()

## Regression Modeling Scores
![scores](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/e048b575-62a5-41db-a66e-0661c1ffd5f3)

**The Best Tuned Model performance on the training data shows an R-squared of 0.604 with a mean square error of 762.69. With the testing data, the model achieved an R-squared of 0.596 and MSE of 737.71.**

**When comparing the training and test scores, we observe that the model performs slightly better on the training data in terms of R-squared. This suggests that the model has successfully learned the underlying patterns in the training data well. There is a small drop in performance on the test data, which is expected as the model encounters new data. This indicates that the model generalizes reasonably well to unseen data and is neither significantly overfit or underfit.**

**Of the modeling performed, the "Best Tuned" model demonstrates a moderately accurate ability to predict product sales, explaining around 60% of the variability in the sales data. The RMSE value of approximately 1056.04 indicates that the model's predictions have an error of around $1,056.04.**

print()
print()
print()


## **Project 1 - Revisited**

**Linear Regression Coefficients**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/88cd30e5-09b3-4754-9556-5f2cda626517)

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/0e8c8045-724e-46db-9d67-b5461724f402)


### LinearRegression Coefficients Explained
- Top three positive coefficients
    - **"Supermarket Type 3" Outlet Type:** An outlet type of "Supermarket type 3" is predicted by our model to increase Outlet_Item_Sales by 600 rupees.
    - **Outlet Identifier 27:**  Store number 27 is predicted by our model to increase Outlet_Item_Sales by 600 rupees.
     - **"Medium" Outlet Size:** Our model predicts that Item_sales increase by about 400 rupees when the outlet is of medium size.
      
print()
print()

**AVERAGE SALES BY OUTLET TYPE**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/728f6e8f-b650-47d2-bbe8-7b022729b2eb)


print()
print()

    

**AVERAGE SALES BY OUTLET IDENTIFIER**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/1e585be4-b688-49e8-b1ce-91d09ed9f417)


- Outlet 27 has the highest average Item Sales.  
- Outlets 10 and 19 have the lowest Item Sales.
  
print()
print()

    


**AVERAGE SALES BY OUTLET SIZE**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/9b07c936-dce8-460b-accc-1e221be4df4f)


- Medium- sized outlets have the highest Item Sales.
- Small outlets tend to have the lowest average sales.  

print()
print()
print()


### Tuned Decision Tree Permutation Feature Importance Explained

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/b3b298f8-3fd9-424b-ade3-61b20bf00f3f)

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/d1a80144-e0fe-4e76-9419-17b50d8d4ed1)

- Top three features
    - **Item MRP (0.74):**   This feature is the highest-weighted feature used by our model to  predict Item Sales.  It is assigned a score of 0.74.
    - **Outlet Type Grocey Store (0.38):** This is the second highest-weighted feature predicted by our model with a score of 0.38.  
    - **Outlet Type Supermarket Type 3 (0.13):**  Outlets of Supermarket Type 3 are predicted to influence the predicted target by a coefficient score of 0.13, ranking this type third highest weighted feature according to the model.
  
print()
print()


**ITEM MRP VS. TOTAL ITEM SALES**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/99b167cd-45e2-4875-b1b2-1d035932ff4a)


- There is a positive trend of increased total item sales as retail price increases.


print()
print()


**OUTLET TYPE VS TOTAL ITEM SALES**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/34932501-8cd4-4d2b-9d17-e1bc938e7e58)

- The figure above shows the average item sales based on Outlet Type.  Supermarket Type 3 has the highest average Item Sales of the four types while Grocery Stores have the lowest averages.  

print()
print()
print()


## Global Explanations with SHAP


- Comparing the figure above with the previous figures for feature and permutation importance, the top three features are consistent across all figures. However, the SHAP average impact of features on the models' predictions slightly differs from the values obtained using the decision tree's built-in feature importance.
- Both SHAP and permutation importance assign slightly less value to Outlet_Type_Grocery_Store, suggesting that the built-in method may have overestimated the importance of this feature in predictions.
- Similarly, the built-in feature importance method may have underestimated the significance of Outlet_Type_Supermarket_Type_3, as it was given slightly higher importance in both the permutation and SHAP summaries


### SHAP Summary

- Item MRP had the most significant impact on our model's predictions. We observe that as the Item MRP value increases, the model is more inclined to predict higher Item Sales.

- For outlets categorized as 'Grocery Store,' our model is more likely to predict lower Item Sales. In our model, Grocery stores have a negative impact on the predicted target.

- Stores classified as 'Supermarket Type 3' tend to have a positive impact on the model's predictions for our target. Therefore, for stores in this category, predicted total item sales are more likely to be higher.

print()
print()
print()



## Local Explanations

### Example 1: Item with Highest MRP

**Examining the item with the highest Maximum Retail Price (MRP) is of particular interest because MRP exhibits a distinct positive correlation with total item sales. In the context of our local explanations, we will delve deeper into this specific example to gain a better understanding of how the highest-priced item contributes to our overall understanding of the sales dynamics**

**EXAMPLE 1: Item with index 945:**

- Has an MRP of 266.18
- Is a Low Fat food
- Canned item type
- Sold at Outlet 13
    - Outlet established in 1987
    - Classified as Supermarket Type 1
    - Location Type of Tier 3
    - High Outlet Size
    
#### Example 1: MRP Force Plot & Lime Explanations 

- SHAPs force plot predicts a base value of 2154 for this item.
    - The highest magnitude contibution came from Item MRP which positively impacted the sales prediction by the model.  
    - Outlet Type Grocey store value of False was the second greatest positive impact on the target value.  
    - The greatest negative impact on sales was the result of the outlet NOT being categorized as Supermarket Type 3 which penalized target value. 
    

- Limes explanations for this instance reflects that if an item has an MRP greater than 182.39, this will push the predicted value in a positive direction. 
    - Grocery Store categorization of false increased the sales prediction by 2008 rupees.
    - Item MRP being greater than 182.39 increased the models target by 1710 rupees.  
 
    
    
    
 ### Example 2: Outlet Type = Grocery Store

**Outlets categorized as 'Grocery Store' tend to have a negative influence on our target variable, our second local explanation example will isolate and analyze an instance related to items sold in grocery stores.**

    **In order to refine our analysis and narrow down the set of items sold in outlets categorized as 'Grocery Store,' we will implement two additional filters. Firstly, we will consider outlets established in 1985, which represents the oldest establishments within our dataset. Secondly, we will incorporate a filter for the item with the highest retail price. By employing these dual filters, our objective is to create a more focused subset of data that can offer us deeper insights into the sales dynamics specific to 'Grocery Store' outlets, especially those that have been in operation for an extended period and involve high-value items.**
 

**Example 2: **Item with index 398:**

- Weight of 12.8 ounces
- MRP of 254.60 Rupees
- Low-fat food
- Sold at Grocery Store number 19
    - Established in 1985
    - Small outlet size
    - Outlet type Tier-1
    
    

#### Expample 2: Grocery Store Force Plot & Lime Explanations

- Our SHAP force plot predicts a base value of 2,154 for this item.  
    - The highest magnitude contribution was Outlet_Type_Grocery Store.  The outlet being categorized as this type of store resulted in the predicted sales being reduced significantly. 
    - Item MRP had the greatest positive contribution to item sales. 
    - Our final predicted sales for this item is estimated to be 604.37 rupees.
    
- Limes explanations for this instance reflects that if an item has an MRP greater than 182.39, this will push the predicted value in a positive direction. 
    - Grocery Store categorization was the largest factor in the predicted price, responsible for reducing the value by 2054 rupees.
    
    
print()

print()

print()

## Recommendations:

TBC


## Limitations & Next Steps

TBC


### For further information


For any additional questions, please contact **chelseycombe@gmail.com**
