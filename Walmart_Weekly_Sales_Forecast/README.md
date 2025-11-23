📈 Walmart Weekly Sales Forecasting
Forecasting weekly sales using historical Walmart data, time-series modeling, and Python. This project analyzes trends, builds a predictive model, and visualizes forecast intervals with upper and lower confidence bounds.

🔍 Project Overview
The goal of this project is to understand Walmart’s weekly sales patterns and build a forecasting model capable of predicting future sales with uncertainty estimates (confidence intervals).
The project includes:
Data cleaning & preparation
Exploratory time-series analysis
Building a mixed effect model to understand what regressors drives sales
Forecasting using Prophet
Generating lower and upper forecast bounds
Combining historical sales data with forecast sales
Exporting final results for Power BI visualization

🛠️ Tools & Technologies
Python (Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Prophet, Sklearn)
Jupyter Notebook
Power BI (for final visualization)
GitHub (project documentation)


/walmart-sales-analysis/
│
├── data/                     # Raw, cleaned & combined datasets
├── plots/                   # Saved Python plots for README + dashboard screenshots
├── walmart_sales_analysis.ipynb   # Complete analysis notebook
├── PowerBI_Dashboard.pbix    # Power BI report 
└── README.md                 # Project documentation

📈 Key Insights 
Weekly sales show strong yearly seasonality, with spikes around major holidays.
Temperature, fuel prices, and CPI have minor influence on sales compared to unemployment.
Stores show similar trends with some stores showing more stable sales pattern.
Forecasts indicate moderate growth.


📊 Exploratory Analysis
Key steps included:
Identifying seasonality in weekly sales
Visualizing historical trends
![Weekly Sales](visuals/weekly_sales_plot.png)

🔮 Forecasting Approach

Model Selection:
1. Linear model with fixed effect which tells us which factors drive sales up or down after controlling for differences between stores. R-squared: 0.920
2. A Prophet model which was extended with external regressors so that the forecast could account for real-world factors that influence sales.
This makes the forecasts more realistic and store-specific.

The forecasts were appended to historical data in Power BI for visualizations
![Power BI Dashboard](visuals/weekly_sales_plot.png)
 
🚀 How to Run

Clone the repo

Install dependencies
pip install -r requirements.txt

Run the notebook
jupyter notebook walmart_sales_analysis.ipynb
