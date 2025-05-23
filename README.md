# Bay Wheels - Bike Rentals Analysis

## Overview

This project investigates real-world data from the Bay Wheels bicycle rental system to uncover the determinants of bike renting activities. By examining hourly usage patterns against weather and time-related factors, the analysis aims to unveil strategic insights. The primary objective is to extract actionable, data-driven conclusions about rider behavior and the influence of environmental circumstances (temperature, humidity, holidays, etc.) on bike usage, ultimately helping Bay Wheels optimize operations, improve customer satisfaction, and plan effectively.

The analysis seeks to answer core business questions such as:
- When and why do riders rent bikes?
- How does weather affect demand for bike rentals?

## Key Findings / Insights

The analysis of the bike rental data provided several key insights into user behavior and influential factors:

1.  *Seasonal Rental Trends:*
    * Rental activity varies significantly across seasons.
    * *Winter:* Experiences slower rental activity, likely due to colder conditions and potential snowfall.
    * *Spring & Summer:* These are peak seasons with the highest average rentals, particularly in the afternoon when weather is most conducive for outdoor activities.
    * *Autumn/Fall:* Shows a gradual decline in rentals as temperatures begin to drop.

2.  *Impact of Temperature on Rentals:*
    * Rentals generally increase with moderate temperatures, with an optimal range observed between *15°C and 25°C*.
    * A sharp decline in rental activity is noted when temperatures drop *below 0°C*.
    * Very high temperatures also tend to reduce rental numbers.

3.  *Hourly Rental Trends & Commuter Patterns:*
    * Two distinct peak rental periods are observed on weekdays: *8–10 AM* (morning rush) and *5–7 PM* (evening rush). This strongly indicates commuter-driven usage for work or school.
    * Rental activity is minimal during late-night and early-morning hours, particularly *between midnight and 5 AM*.

4.  *Influence of Other Weather Conditions:*
    * *Humidity:* Rentals tend to decrease when humidity exceeds 80%. The ideal humidity range for higher rental volumes appears to be between 40%-60%.
    * *Wind Speed:* Higher wind speeds show a slight negative correlation with the number of rentals.
    * *Rainfall & Snowfall:* Both rainfall and snowfall have a negative correlation with bike rentals, indicating that precipitation drastically reduces usage.

## Methodology & Technologies Used

*Methodology:*
The project employs a quantitative-qualitative mixed method to interpret trends in hourly bicycle rentals. This involves analyzing patterns based on time of day, seasonality, and various weather conditions. The report aims to be stakeholder-friendly by incorporating storytelling and clear visualizations.

*Technologies Used:*
* *Python:* The core language used for data analysis.
* *Pandas:* For data manipulation and analysis, including reading the dataset from an Excel file.
* *Matplotlib & Seaborn:* For creating visualizations such as bar plots, scatter plots, line plots, and heatmaps to illustrate trends and correlations.

## Dataset

The analysis is based on a dataset named bikes_data.xlsx. The dataset contains hourly bike rental records with the following key features:
* ID
* Month
* Day of Week
* Hour
* Temperature (°C)
* Humidity (%)
* Wind Speed (m/s)
* Visibility (m)
* Dew Point Temperature (°C)
* UV Index
* Rainfall (mm)
* Snowfall (cm)
* Season (Winter, Spring, Summer, Autumn)
* Holiday (Yes/No)
* RENTALS (Number of bike rentals)

## How to Run

1.  Ensure you have Python installed along with the necessary libraries: pandas, matplotlib, and seaborn.
    bash
    pip install pandas matplotlib seaborn openpyxl
    
2.  Place the dataset file bikes_data.xlsx in the same directory as the Jupyter Notebook (A2 - Python Analysis Project -Individual-.ipynb).
3.  Open and run the Jupyter Notebook using an environment like Jupyter Lab or Jupyter Notebook.

## Analysis Questions & Recommendations (Summary)

*1. Why are the majority of users renting bicycles?*
   The data strongly suggests that most users rent bicycles for *commuting purposes* (e.g., to work or school), as evidenced by peak rental hours on weekdays (8–10 AM and 5–7 PM). Leisure or casual riding appears to be less common.

*2. Are there any ideal weather conditions for high demand?*
   Yes, *moderate temperatures (15°C–25°C), dry conditions, and **low humidity (40%-60%)* are ideal for bike rentals. Extreme temperatures, high humidity, and precipitation significantly deter riders.

*3. How should the company plan based on these findings?*
    * *Optimize Fleet Deployment:* Increase bike availability during weekday peak commuter hours and in favorable weather conditions. Reduce availability during late nights, off-peak seasons, and poor weather.
    * *Targeted Promotions:*
        * Launch real-time, weather-based promotions on good weather days.
        * Offer incentives for morning/evening commuters.
        * Provide discounts on low-demand days or during marginally adverse weather to encourage usage.
    * *Operational Efficiency:* Use predictive demand modeling (based on weather, time, season) to optimize staffing and maintenance schedules, thereby reducing costs.
    * *Strategic Partnerships:* Consider corporate alliances to target working professionals during peak commute times.

## References
* El-Assi, W., Mahmoud, M. S., & Habib, K. N. (2017). Effects of built environment and weather on bike sharing demand: A station level analysis of Toronto. Transportation, 44(3), 589–613.
* Fishman, E., Washington, S., & Haworth, N. (2014). Bike share: A synthesis of the literature. Transport Reviews, 33(2), 148–165.
* Gebhart, K., & Noland, R. B. (2014). The impact of weather conditions on bikeshare trips in Washington, DC. Transportation, 41(6), 1205–1225.
* Shaheen, S., Guzman, S., & Zhang, H. (2012). Bikesharing across the globe. Transportation Research Record: Journal of the Transportation Research Board, 2314(1), 159–167.
* Lecture notes (Python Class by Professor Chase).
