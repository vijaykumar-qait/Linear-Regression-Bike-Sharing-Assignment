# Linear Regression Bike Sharing
> The Corona epidemic has caused dramatic revenue declines for US bike-sharing company BoomBikes. 
> The company has created a business plan to better grasp the demand for shared bikes following a pandemic in order to bounce back 
> Once the situation gets better, the scheme seeks to meet people's needs and generate notable profits. 
> The corporation will borrow bikes from docks under computer control and bring them back to another pier.

# Business Goal:
> Once the Covid-19 quarantine ends, BoomBikes wants to know how much demand shared bikes create in the American market. 
> BoomBikes hires a consultancy firm to identify key variables and understand the factors influencing demand. 
> By means of meteorological surveys and people's preferences, compile a report on daily bike needs over the American market. 
> By modeling the need for shared bikes with independent variables, managers can modify their business plan to satisfy consumer demand and customer expectations.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This project aims to develop a Multiple Linear Regression model to forecast shared bike demand within a bike-sharing system. 
- The project intends to maximize the business plan for a bike-sharing firm and grasp all factors impacting the rental count.

## Data Set Applied
- This study makes use of a U.S. bike-sharing system's dataset. It covers details on daily bike rentals, the state of the weather, time-related characteristics, and whether today is a working day or a holiday.
- The primary features consist in:
Overall rental count (target variable)
Dates: Year, Month, Weekday, Season
- Temperatures, humidity, wind speed, weather conditions:
Working Day, Holiday: Type Indicator Day



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## **Key Findings & Conclusions**
### **1. Temperature Strongly Affects Bike Rentals**  
- Higher temperatures lead to increased bike demand.  
- Extreme weather (heavy rain or snow) significantly reduces rentals.  

### **2. Increasing Trend in Bike Rentals Over Time**  
- The **year-over-year trend** indicates growing adoption of bike-sharing services.  
- Bike rentals in **2019 were significantly higher than in 2018**, showing increased customer preference.  

### **3. Seasonal Impact on Demand**  
- **Peak season:** **Summer and fall** have the highest rental counts.  
- **Low season:** **Spring and winter** show a noticeable drop in demand.  
- Seasonal variations suggest that biking is **preferred in moderate and warm weather conditions**.  

### **4. Negative Impact of Wind Speed & Humidity**  
- Higher **humidity** discourages bike rentals, possibly due to discomfort.  
- Strong **winds** reduce rentals, likely due to difficulty in riding.  

### **5. Weekends & Holidays Show Different Rental Patterns**  
- **Working days still see significant bike rentals**, indicating heavy usage for **commuting**.  
- **Weekends & holidays** exhibit different demand patterns, likely due to leisure biking.  

### **6. Feature Selection & Model Optimization**  
- **Recursive Feature Elimination (RFE) + Variance Inflation Factor (VIF)** were used to remove **multicollinearity** and select the best predictors.  
- Unnecessary variables like **‘atemp’ (adjusted temperature)** were dropped due to their **high correlation with temperature**.  

### **7. Handling Outliers for Better Model Accuracy**  
- Extreme values in **temperature, humidity, and wind speed** were **removed using IQR filtering**.  
- This helped improve model stability and accuracy.  

### **8. Strong Model Performance**  
- **Train R²:** **0.84** | **Test R²:** **0.83** → The model generalizes well without overfitting.  
- **Mean Absolute Error (MAE):** **~578**  
- **Root Mean Squared Error (RMSE):** **~803**  
- The model has **good predictive power** and captures demand variations effectively.  

### **9. Model Assumption Validations**  
✅ **Normality of Residuals:** Checked using **Q-Q plots and histograms**. Residuals follow a **normal distribution**.  
✅ **No Multicollinearity:** Verified using **VIF analysis**, ensuring independent variables do not have strong correlations.  
✅ **Homoscedasticity Confirmed:** **Residual plots** show no systematic pattern, proving that variance remains constant.  

## **Business Implications**
🚲 **Optimized Bike Distribution:** Companies can **allocate bikes efficiently** based on predicted demand in different seasons and weather conditions.  
🚲 **Seasonal Pricing Strategies:** Adjusting **rental pricing** based on peak and low-demand seasons can maximize profits.  
🚲 **Weather-Based Forecasting:** Integrating **real-time weather data** can improve **demand predictions** and **inventory management**.  
🚲 **Expansion Opportunities:** The **growing trend in bike rentals** suggests **potential business growth**, encouraging further investment in bike-sharing infrastructure.  


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Pandas (v1.3.3) - Data manipulation and analysis
- NumPy (v1.21.2) - Numerical computing
- Matplotlib (v3.4.3) - Data visualization
- Seaborn (v0.11.2) - Statistical data visualization
- Scikit-learn (v1.0) - Machine learning and preprocessing
- Statsmodels (v0.13.2) - Statistical modeling and regression analysis
- Warnings (built-in) - Suppress warnings in output



<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
This project is inspired by real-world demand forecasting challenges faced by bike-sharing companies. The dataset is based on a publicly available dataset from bike-sharing systems in the U.S.
References:
This project was influenced by machine learning best practices in linear regression.
Data and problem statement inspired by BoomBikes case study.
Additional guidance was taken from Scikit-learn and Statsmodels documentation.


## Contact
Created by [@vijaykumar-qait] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->