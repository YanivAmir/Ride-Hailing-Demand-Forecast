14/08/2024

Ride Hailing Demand Forecasting and Linear Surge Cost Model

A time-series anlysis for sample data in the ride-hailing marketplace.
The goal was to find ways to bridge supply and demand more efficiently using forecasting for expected demand.

Tech used:

<img alt="Python" src="https://img.shields.io/badge/Python-3776ab?logo=python&logoColor=white&style-flat"><img alt="Pytorch" src="https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white&style-flat">
<img alt="scikit-learn" src="https://img.shields.io/badge/Scikit-f7931e?logo=scikit-learn&logoColor=white&style-flat">
<img alt="NumPy" src="https://img.shields.io/badge/NumPy-013242?logo=numpy&logoColor=white&style-flat">
<img alt="Pandas" src="https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white&style-flat">
<img alt="GeoPandas" src="https://img.shields.io/badge/GeoPandas-139c5a?logo=GeoPandas&logoColor=white&style-flat">
<img alt="Jupyter" src="https://img.shields.io/badge/Jupyter-f37626?logo=jupyter&logoColor=white&style-flat">

The script includes:
Exploratory data analysis, data cleaning, feature design, 
Exponential moving average (EMA) and LSTM models for demand predicition, both preform equally well (though I admit I ddin't invest too much in optimizing them)
A dynamic surge cost model, both linear and exponential,
A/B testing description.

SampleData uploaded contains 80% of original data, so results may differ slightly from the results shown.

#### The aggregated demand map for the entire 28-day duration, geogrpahically distributed. 
![image](https://github.com/user-attachments/assets/05280818-7916-432a-a6c9-b3a416c9abc2)

#### The X axis is the hexagon density plot with the 35x35 hexgrid flattened to a vector. Most of the hexes are low demand areas, which stay in low demand throughout the entire data period. 
![image](https://github.com/user-attachments/assets/256cc254-b8c7-4783-9562-61613dd70173)

#### The prediction vs true demand values for the LSTM model for the final 130hrs of the top 5 locations in highest demand:
![image](https://github.com/user-attachments/assets/83155419-15c7-4293-ab2e-9d94229d6ae5)

#### Map displays with the integrated linear surge cost for the EMA model:
![image](https://github.com/user-attachments/assets/7a23e4b3-dd2a-4cfd-ac75-391a7a642ae0)

