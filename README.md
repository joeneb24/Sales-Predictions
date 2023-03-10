# Sales Predictions

![image](https://user-images.githubusercontent.com/123125444/224272426-d439f3d5-ba4b-4ea9-8904-8fdbf315454f.png)

# Analyzing and Predicting Store Products Sales 
Many times it is hard to tell if a certain product is going to sell at the expect price or quantity. This information is vital in knowing what products need to be reworked or change in product placement. All of these factors account for the overall success in a business that is selling items on shelves. 

# Data Dictionary
![image](https://user-images.githubusercontent.com/123125444/224272935-fd34b7d7-3de0-4ef0-9091-5241bb8c7258.png)

# Data preparation and cleaning was done on the data before the following processes:

## Exploratory Data Analysis
- The figure below is a histogram that shows the distribution of the Item Outlet Sales of the different items sold. This data shows that there are more items sold that have lower item outlet sales. The figure also shows the median of the item outlet sales which is $1,794.33 and is designated with the dashed line. 
![image](https://user-images.githubusercontent.com/123125444/224275509-cf563772-09e2-4d91-bc34-d36a046444aa.png)

- The figure below shows that there are more unique Low Fat items that there are Regular items that are available.
![image](https://user-images.githubusercontent.com/123125444/224276329-d52328e3-7e1d-4f50-8446-b33de37cabe4.png)

- The figure below shows that the only sets of data that have any sort of correlation are Item_Visibility and Item_Outlet_Sales. The correlation is a negative correlation, so as Item_Visibility goes up, the Item_Outlet_Sales goes down, and vice versa.
![image](https://user-images.githubusercontent.com/123125444/224287372-ef3c0e77-b642-464d-830f-8ecef3a63d73.png)

## Explanatory Data Analysis
- In the visual above, we see that the item visibility avearge is 0.066 and its median is 0.054. Most of the item visibility is low across the board.
![image](https://user-images.githubusercontent.com/123125444/224277000-062c2395-df41-44b5-98b0-79281fce7962.png)

## Maching Learning Using the Following Models:
- Linear Regression Model
- Random Forest Regressor Model
- Tuned Random Forest Regressor Model

## Models Evaluated & Results:

Linear Regression Model:
- Linear Regression Train Scores:
  * MAE: 847.1288  
  * MSE: 1,297,558.1288  
  * RMSE: 1,139.1041 
  * R2: 0.5616
  
- Linear Regression Test Scores:
  * MAE: 804.1203
  * MSE: 1,194,349.9312 
  * RMSE: 1,092.8632 
  * R2: 0.5671
  
Tuned Random Forest Model:
- Linear Regression Train Scores
  * MAE: 293.3091 
  * MSE: 176,253.5394 
  * RMSE: 419.8256 
  * R2: 0.9404

- Linear Regression Test Scores
  * MAE: 767.5726 
  * MSE: 1,215,938.3653 
  * RMSE: 1,102.6960 
  * R2: 0.5593
  
- The final model chosen was the linear regression model for the following reasons:
  * Overall, the best model is definitely the linear regression model. There were still some bias on the data, but compared to the high variance in the random forest model, it showed that it could better perform at predicting outlet sales. This is very apparent when comparing the differences in the training data's prediction outlet sales when comparing the RMSE. The linear regression model predicted the outlet sales within $47.
  * As compared with the TUNED random forest model, the model was off by $683.
  * Becuase of these highlighted reason, I recommend the linear regression model over the random forest model in predicting outlet sales.
  
# Key Insights
- Both of the histograms above have similar shapes. We can see that high visibility items are quite low in count. We also see that the higher the item outlet sales, the count of item are being sold at that higher price. 
- We also see that the store carries more low fat items in the stores. 
- From the heat map above, we also see that most of the data features do not have a lot or correlation between each other, making it harder to predict testing data. We may need more data to work with or add new features to the data to better predict sales. 
- From the data, we can predict item outlet sales using linear regression models, but 
  
# Final Recommedation
- We may need more data and more data features for better sales predictions, but if we needed to predict sales now the linear regression model work the best. 
  
  
  
  
  
  
  
  
