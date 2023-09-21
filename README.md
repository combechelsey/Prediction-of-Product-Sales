# Prediction-of-Product-Sales
## Predicting Trends of Item Sales Across an Array of Grocery Outlets

**Chelsey Combe**: 

### Business problem:

Employing Regression Modeling to Forecast Item Sales and Illuminate the Formula for Success for Grocery Stores and Supermarkets!


### Data:

![image](https://github.com/combechelsey/Prediction-of-Product-Sales-2/assets/132314345/13915534-615b-4c29-81f9-329c9cb9c6ee)

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




## **Project 1 - Revisited**

**Linear Regression Coefficients**
![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/498250c3-661b-4514-9784-3ca29fa7de3a)

### LinearRegression Coefficients Explained
- Top three positive coefficients
    - **"Supermarket Type 3" Outlet Type:** This feature has the highest positive correlation on Item Sales.  A "Supermarket Type-3" outlet is associated with higher sales. 
    - **Outlet Identifier 27:** This particular store is positively correlated with our target and item sales tend to be higher at this location. 
    - **"Medium" Outlet Size:** Outlets with a medium size tend to have higher sales compared to small or large outlet sizes. 

      
- Top three negative coefficients        
    - **"Grocery Store" Outlet Type:** this classification has the strongest negative correlation and is associated with lower sales. Customers typically buy less in grocery stores compared to other types of outlets according to this model.
        
    - **Outlet Identifier 19:**  Specifically, the outlet with the identifier "OUT019" has a significant negative correlation with sales. Sales tend to be lower in this particular outlet.
    - **Outlet Identifier 19:**  Similar to above, Outlet 10 also negatively correlates with sales and suggest that this outlet may also underperform in terms of sales.


![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/65b2e607-3d72-45e3-8731-e54dda88e942)

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/fa2ca2f1-aaf0-43c2-8668-4aefb731db66)

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/8729b53c-03b9-4468-9946-73863b0bd608)

**XGBoost Feature Importance**

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/d0293518-7221-4a38-81cf-3bf8c8ecd8fc)


### XG Boost Permutation Feature Importance Explained
- Top three features
    - **Item MRP (1.01):** This model predicts that for every dollar change in MRP, Item sales increase or decrease by 1.01 units.   
    - **Outlet Establishment Year (0.21):** This particular store is positively correlated with our target and item sales tend to be higher at this location. For each year in age of the outlet, item sales decrease by 0.22 units.  
    - **Item Weight (0.14):** Outlets with a medium size tend to have higher sales compared to small or large outlet sizes.  For each ounce in an tems weight, item sales increase or decrease by 0.15 units.
  
![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/37dfe9ba-02c2-468a-a853-be88fbf79b32)

![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/f28325a5-e666-4d30-9504-f98a2c78a0ce)


![Untitled](https://github.com/combechelsey/Prediction-of-Product-Sales/assets/132314345/85ddd0eb-a653-4a5e-8180-c1c6cef373fa)








## Recommendations:

TBC


## Limitations & Next Steps

TBC


### For further information


For any additional questions, please contact **chelseycombe@gmail.com**
