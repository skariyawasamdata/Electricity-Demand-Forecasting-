#  Electricity Demand Forecasting

This project focuses on predicting electricity demand using historical data and time series forecasting techniques. Accurate forecasting helps in efficient energy management and planning.



##  Project Overview
Electricity demand forecasting is essential for:
* Power generation planning
* Load management
* Reducing energy waste

This project uses data analysis and machine learning (specifically **XGBoost**) to forecast future electricity demand.



##  Tools & Technologies
* **Python**: Core programming language
* **Pandas & NumPy**: Data manipulation
* **Matplotlib & Seaborn**: Data visualization
* **Scikit-learn**: Machine learning utilities
* **XGBoost**: Gradient boosted decision trees for forecasting

---

## Exploratory Data Analysis (EDA)

### Historical Demand Over Time
![Electricity Demand Over Time](images\Electricity Demand Over Time.png)

*Historical consumption patterns from 2020 through early 2025 showing clear seasonality.*

### Demand Drivers & Correlations
![Correlation Matrix](images\correlation Matrix of features.png)
*The correlation matrix reveals a strong positive relationship ($0.83$) between **Temperature** and **Demand**.*

### Seasonality & Trends
| Hourly Trends | Monthly Trends |
| :--- | :--- |
| ![Demand by Hour](images\Demand by Hour of the day.png) | ![Demand by Month](images\Demand by month.png) |
| *Demand peaks during midday and evening hours.* | *Higher demand is observed during summer months (June–August).* |

### Temperature Impact
![Demand vs Temperature](images\Demand Vs Temperature.png)
*A scatter plot visualizing how demand scales upward as temperatures increase.*

---

## Model & Results
We utilized an **XGBoost regressor** to predict demand based on temporal features and weather data.

### Prediction Performance
![XGBoost Prediction](images\XGBoost Electricity Demand Prediction.png)
*The model (red dashed line) closely follows the actual demand (blue line), capturing both daily cycles and seasonal peaks.*

---

##  Project Structure
* `data/`: Raw and processed datasets.
* `images/`: Exported visualizations used in this README.
* `models/`: Saved model weights/pickles.