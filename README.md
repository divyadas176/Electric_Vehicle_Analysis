# Electric Vehicle Specifications and Prices

### Project Overview
This project explores the "Electric Vehicle Specifications and Prices" dataset, providing a detailed analysis of electric vehicles available in the market. The dataset contains **360 entries and 9 variables**, covering aspects such as battery capacity, model name, efficiency, fast-charging capabilities, pricing in Germany, range, top speed, and acceleration from 0–100 km/h.

The goal of this project is to **perform data cleaning, exploratory data analysis (EDA), and visualization** to uncover patterns and insights related to EV performance and pricing.

---

### Dataset Description
The dataset was collected from [EV Database](https://www.kaggle.com/datasets/fatihilhan/electric-vehicle-specifications-and-prices), a leading source of electric vehicle information. Each record includes:

- **Battery**: Battery capacity in kilowatt-hours (kWh)  
- **Model**: Vehicle model name  
- **Link**: Link to the EV Database for more information  
- **Efficiency**: Vehicle efficiency ratings  
- **Fast-Charging**: Whether fast charging is supported  
- **Price**: Vehicle price in Germany  
- **Range**: Driving range per full charge (km)  
- **Top Speed**: Maximum speed of the vehicle (km/h)  
- **Acceleration**: 0–100 km/h acceleration time (seconds)  

---

### Analytical Objectives & Research Questions
To guide this analysis, the project focused on answering three core research questions:

- Is the German EV market dominated by budget-friendly options or luxury performance models?
- What is the distribution of battery capacities among EVs, and do most vehicles cluster around specific battery size ranges?
- What is the distribution of driving ranges among electric vehicles, and do most EVs cluster around specific range intervals?
- What is the nature and strength of the relationship between battery capacity and driving range in electric vehicles?
- How does the price of electric vehicles relate to their driving range?
- How does the price of electric vehicles relate to their top speed?
- To what extent does vehicle efficiency act as a mediating factor between battery capacity and real-world range across different manufacturer segments?
- Does paying a premium for an electric vehicle in Germany guarantee a more energy-efficient powertrain, or is high price primarily driven by battery size and      luxury features?
- When you buy an expensive EV, are you actually paying for the convenience of faster charging, or is fast charging just a standard feature that comes with a bigger battery?
- Does a bigger battery always mean faster charging, or are some cars just engineered better to charge quickly?
- Does a faster acceleration time (0–100 km/h) justify a higher market price in Germany, or is it merely a side effect of larger, more expensive battery packs?
- How does the average Price_per_km compare across the Top 10 manufacturers in the 2024 German market, and which brand offers the most "range for the Euro"?

---
  
### Project Goals
- Clean and preprocess the dataset for analysis  
- Explore distributions and relationships between features (battery, range, price, etc.)  
- Visualize trends in performance, pricing, and efficiency  
- Provide actionable insights for EV enthusiasts, buyers, and researchers  

---

### Usage
- The notebook `Electric_Vehicle_Analysis.ipynb` contains the full analysis, including plots and insights.  
- To reproduce the results, simply open the notebook in Jupyter or Google Colab and run the cells.  

---

### Insights
- The "Mass-Market" Sweet Spot: While luxury EVs exist, the German market is dominated by a high-density "Value Cluster" priced between €40,000 and €70,000. This suggests that manufacturers are prioritizing mid-range affordability for mass adoption.
- Impact of Outliers: Initial analysis was heavily skewed by luxury models (over €115,000). Removing these outliers revealed a much more consistent and reliable $R = 0.74$ correlation between Range and Price for the average consumer.
- Charging Efficiency vs. Size: Battery size acts as a technical enabler for speed, but a "vertical surge" at the 75–85 kWh mark proves that superior engineering (like 800V architecture) allows some mid-sized batteries to outcharge larger, more expensive ones.
- The Performance Premium: There is a clear "Luxury Ceiling" where price increases exponentially not for range, but for acceleration (0–100 km/h) and brand prestige, indicating that speed remains a primary differentiator for high-end models.
- Hardware Bottlenecks: Correlation heatmaps confirmed that fast-charging speeds are physically tied to battery capacity (kWh), identifying ultra-fast charging as a "hardware-locked" premium feature in the current market.  

---

## Author
- Divya Das  
- Data analysis and visualization using Python (Pandas, Seaborn, Matplotlib)  
