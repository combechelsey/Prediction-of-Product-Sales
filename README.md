# Prediction-of-Product-Sales
## Predicting Trends of Item Sales Across an Array of Grocery Outlets

**Chelsey Combe**: 

### Business problem:

Employing Regression Modeling to Forecast Item Sales and Illuminate the Formula for Success for Grocery Stores and Supermarkets!


### Data:

![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/13915534-615b-4c29-81f9-329c9cb9c6ee)
/n
/n
/n

## Methods
- Inspected and cleaned data by removing duplicate values, standardizing value counts, explored data outliers, and modified data to correctly assign datatypes.  
- Created univariate and multivariate visualizations to further analyze the overall trends of the dataset.
- Prepare data for Machine Learning modeling.
- Used various regression modeling techniques to gather regression metric data and correlations between features.  

## Results

#### Classification of Items Inclued in Analysis 
![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/1ffb9905-dae4-472b-9c42-bf7ad4297583)


#### Outlet Sales by Item Type
![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/03872d47-815e-462b-9a16-c858d51e3640)


#### Total Item Sales by Outlet Size
![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/0f38ad9b-841b-4d06-a992-ae338b3d483e)

#### Total Item Sales by Outlet Type
![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/f5088429-5a28-443b-ad32-df30cf46284b)


## Regression Modeling Scores
![scores](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/e048b575-62a5-41db-a66e-0661c1ffd5f3)

**The Best Tuned Model performance on the training data shows an R-squared of 0.604 with a mean square error of 762.69. With the testing data, the model achieved an R-squared of 0.596 and MSE of 737.71.**

**When comparing the training and test scores, we observe that the model performs slightly better on the training data in terms of R-squared. This suggests that the model has successfully learned the underlying patterns in the training data well. There is a small drop in performance on the test data, which is expected as the model encounters new data. This indicates that the model generalizes reasonably well to unseen data and is neither significantly overfit or underfit.**

**Of the modeling performed, the "Best Tuned" model demonstrates a moderately accurate ability to predict product sales, explaining around 60% of the variability in the sales data. The RMSE value of approximately 1056.04 indicates that the model's predictions have an error of around $1,056.04.**

/n
/n
/n


## **Project 1 - Revisited**

**Linear Regression Coefficients**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/88cd30e5-09b3-4754-9556-5f2cda626517)

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/0e8c8045-724e-46db-9d67-b5461724f402)


### LinearRegression Coefficients Explained
- Top three positive coefficients
    - **"Supermarket Type 3" Outlet Type:** An outlet type of "Supermarket type 3" is predicted by our model to increase Outlet_Item_Sales by 600 rupees.
    - **Outlet Identifier 27:**  Store number 27 is predicted by our model to increase Outlet_Item_Sales by 600 rupees.
     - **"Medium" Outlet Size:** Our model predicts that Item_sales increase by about 400 rupees when the outlet is of medium size.
      
/n
/n

**AVERAGE SALES BY OUTLET TYPE**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/728f6e8f-b650-47d2-bbe8-7b022729b2eb)


/n
/n

    

**AVERAGE SALES BY OUTLET IDENTIFIER**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/1e585be4-b688-49e8-b1ce-91d09ed9f417)


- Outlet 27 has the highest average Item Sales.  
- Outlets 10 and 19 have the lowest Item Sales.
  
/n
/n
    


**AVERAGE SALES BY OUTLET SIZE**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/9b07c936-dce8-460b-accc-1e221be4df4f)


- Medium- sized outlets have the highest Item Sales.
- Small outlets tend to have the lowest average sales.  

/n
/n
/n 


### Tuned Decision Tree Permutation Feature Importance Explained

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/b3b298f8-3fd9-424b-ade3-61b20bf00f3f)

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/d1a80144-e0fe-4e76-9419-17b50d8d4ed1)

- Top three features
    - **Item MRP (0.74):**   This feature is the highest-weighted feature used by our model to  predict Item Sales.  It is assigned a score of 0.74.
    - **Outlet Type Grocey Store (0.38):** This is the second highest-weighted feature predicted by our model with a score of 0.38.  
    - **Outlet Type Supermarket Type 3 (0.13):**  Outlets of Supermarket Type 3 are predicted to influence the predicted target by a coefficient score of 0.13, ranking this type third highest weighted feature according to the model.
  
/n
/n

**ITEM MRP VS. TOTAL ITEM SALES**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/99b167cd-45e2-4875-b1b2-1d035932ff4a)


- There is a positive trend of higher Item Sales as Item MRP increases.

/n
/n

**OUTLET TYPE VS TOTAL ITEM SALES**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/34932501-8cd4-4d2b-9d17-e1bc938e7e58)

- The figure above shows the average item sales based on Outlet Type.  Supermarket Type 3 has the highest average Item Sales of the four types while Grocery Stores have the lowest averages.  

/n
/n
/n

## Recommendations:

TBC


## Limitations & Next Steps

TBC


### For further information


For any additional questions, please contact **chelseycombe@gmail.com**
