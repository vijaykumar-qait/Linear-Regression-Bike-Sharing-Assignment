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

## Conclusions
- Temperature has the highest positive correlation with bike demand. Warmer temperatures result in higher rentals, while extreme weather conditions (heavy rain or snow) decrease demand.
- Year (trend effect) shows increasing bike rentals over time, indicating growing popularity.
- Seasonal variations exist: Rentals are highest in summer and fall and lowest in spring.
- Wind speed and humidity negatively impact demand, with higher wind speed or humidity leading to fewer bike rentals.
- Weekends and holidays have different rental patterns, but working days still see a significant number of rentals.
- Feature selection (RFE + VIF) was performed to remove multicollinearity and improve model performance.
- The final model shows an R-squared value of ~0.81, indicating a strong predictive ability.

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