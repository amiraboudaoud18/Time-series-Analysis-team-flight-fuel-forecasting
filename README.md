# ✈️ Team Flight Fuel Forecasting 2102 usin Time Series Analaysis 
![team flight fuel forecasting image](./baseball_flights.png)


This project analyzes team flight data and jet fuel prices from the year 2101 to support **logistics planning** and **budget forecasting** for 2102. Using real-world time series modeling and data manipulation techniques, we:

- Determined the **maximum number of teams in flight at the same time**
- **Forecasted fuel prices** for 2102 using SARIMAX models
- **Estimated the total fuel spend** for all team flights in 2102


## 📊 Project Overview

### Goals
1. Analyze team travel schedules to understand peak air traffic.
2. Model and forecast daily jet fuel prices using time series techniques.
3. Calculate projected flight costs for 2102 using the forecasted prices.

### Tools & Technologies
- **Python**, **Pandas**, **NumPy**
- **Statsmodels** (SARIMAX time series modeling)
- **Matplotlib** for visualization
- **Jupyter Notebook**

## 🚀 How It Works

### Step-by-Step Workflow

1. **Data Cleaning**:
   - Parsed and formatted datetime columns from flight data.
   - Converted fuel price index to a proper time series format.

2. **Simultaneous Flights Analysis**:
   - Combined all departure and landing events.
   - Counted how many teams were flying at any given moment.
   - Visualized flight concurrency over time.

3. **SARIMAX Forecasting**:
   - Modeled jet fuel prices using `(1,1,1)` order and `(1,0,0,7)` seasonal order.
   - Forecasted daily prices for 2102.

4. **Fuel Spend Estimation**:
   - Merged predicted fuel prices with team flight data by departure date.
   - Multiplied travel distance by forecasted price per day.
   - Summed all flight costs to calculate the **total projected fuel spend** for 2102.

---

## 📁 Project Structure
- team_flights.csv # Dataset of team flight schedules
- fuel_prices_2101.csv # Historical daily fuel prices for 2101
- notebook.ipynb # Main analysis notebook
- EADME.md # Project documentation


## 📌 Key Results
- **Maximum Simultaneous Flights:** 19  
- **Projected Fuel Spend for 2102:** ~ **$2.1 million** (based on SARIMAX predictions)


## 📚 Learnings & Highlights
- How to detect and visualize **temporal overlap** in scheduling data.
- Application of **SARIMAX** to model trend + weekly seasonality in pricing.
- Joining time series forecasts with real-world event data to produce **business insights**.


## 🧠 Future Work
- Incorporate external features (e.g. weather, demand) into forecasting.
- Consider varying flight costs based on aircraft or fuel efficiency.
- Create interactive dashboards with Plotly or Streamlit.
