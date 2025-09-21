# 🌾 Weather and Soil Index-Based Crop Insurance using Regression Analysis and EWM-TOPSIS

## 📝 Overview
This repository contains the code and analysis for the research project, **"Weather and Soil Index Based Crop Insurance using Regression Analysis and EWM-TOPSIS"**.  
The study proposes a novel weather and soil index-based crop insurance scheme for wheat in three Indian states: **Uttar Pradesh, West Bengal, and Bihar**.  

By integrating key weather and soil variables, the model develops **state-specific insurance contracts** designed to minimize basis risk and provide more accurate compensation to farmers.

---

## ✨ Key Features
- **State-Specific Models**: Develops unique insurance contracts for West Bengal, Uttar Pradesh, and Bihar based on their specific agricultural risks.  
- **Multi-Factor Index**: Incorporates rainfall, temperature, NPK consumption, and net irrigated area into a robust insurance index.  
- **Hybrid Methodology**: Combines regression analysis (to identify key risk factors) with **EWM-TOPSIS** (to validate and assign objective weights).  
- **Data-Driven Design**: Reduces **basis risk** (when farmers suffer losses but don’t get payouts) by ensuring the index is strongly correlated with actual yield losses.  

---

## 🛠️ Methodology
1. **Data Collection & Preprocessing**  
   - Historical data (2005–2024) for wheat yield, rainfall, temperature, NPK consumption, and irrigated area.  
   - Wheat yields detrended using **robust regression (Bisquare & Huber)** to remove time influence.  

2. **Regression Analysis**  
   - Detrended yields regressed on weather and soil variables.  
   - Identified the most significant factors per state.  

3. **EWM-TOPSIS Validation**  
   - **Entropy Weight Method (EWM)** → objective weights from variability.  
   - **TOPSIS** → ranked years by risk, validating selected indices.  

4. **Insurance Contract Design**  
   - State-specific indemnity contracts with triggers, exit levels, and payouts.  
   - **Pure Premium Rates (PPR)** calculated for fair premiums.  

---

## 📊 Results
The analysis identified the most critical factors for each state:

- **West Bengal**: Rainfall + Net Irrigated Area → PPR: **3.48%**  
- **Uttar Pradesh**: Temperature + Rainfall → PPR: **5.68%**  
- **Bihar**: Net Irrigated Area + NPK Consumption → PPR: **7.64%**  

---

## 📂 Repository Structure
# 🌾 Weather and Soil Index-Based Crop Insurance using Regression Analysis and EWM-TOPSIS

## 📝 Overview
This repository contains the code and analysis for the research project, **"Weather and Soil Index Based Crop Insurance using Regression Analysis and EWM-TOPSIS"**.  
The study proposes a novel weather and soil index-based crop insurance scheme for wheat in three Indian states: **Uttar Pradesh, West Bengal, and Bihar**.  

By integrating key weather and soil variables, the model develops **state-specific insurance contracts** designed to minimize basis risk and provide more accurate compensation to farmers.

---

## ✨ Key Features
- **State-Specific Models**: Develops unique insurance contracts for West Bengal, Uttar Pradesh, and Bihar based on their specific agricultural risks.  
- **Multi-Factor Index**: Incorporates rainfall, temperature, NPK consumption, and net irrigated area into a robust insurance index.  
- **Hybrid Methodology**: Combines regression analysis (to identify key risk factors) with **EWM-TOPSIS** (to validate and assign objective weights).  
- **Data-Driven Design**: Reduces **basis risk** (when farmers suffer losses but don’t get payouts) by ensuring the index is strongly correlated with actual yield losses.  

---

## 🛠️ Methodology
1. **Data Collection & Preprocessing**  
   - Historical data (2005–2024) for wheat yield, rainfall, temperature, NPK consumption, and irrigated area.  
   - Wheat yields detrended using **robust regression (Bisquare & Huber)** to remove time influence.  

2. **Regression Analysis**  
   - Detrended yields regressed on weather and soil variables.  
   - Identified the most significant factors per state.  

3. **EWM-TOPSIS Validation**  
   - **Entropy Weight Method (EWM)** → objective weights from variability.  
   - **TOPSIS** → ranked years by risk, validating selected indices.  

4. **Insurance Contract Design**  
   - State-specific indemnity contracts with triggers, exit levels, and payouts.  
   - **Pure Premium Rates (PPR)** calculated for fair premiums.  

---

## 📊 Results
The analysis identified the most critical factors for each state:

- **West Bengal**: Rainfall + Net Irrigated Area → PPR: **3.48%**  
- **Uttar Pradesh**: Temperature + Rainfall → PPR: **5.68%**  
- **Bihar**: Net Irrigated Area + NPK Consumption → PPR: **7.64%**  

---

## 📂 Repository Structure
````.
├── Code/             # Jupyter notebooks for analysis
│   ├── 1_assumptionscheck.ipynb
│   ├── 2_ewmtopsis.ipynb
│   └── 3_premium.ipynb
│   └── 3_regression.ipynb
├── Data/                  # Raw and preprocessed datasets (.csv)
│   ├── 1_Bihar/
│   │   ├── 1_finalcompileddatabihar.csv
│   │   ├── 2_finalcompileddatabihar.xlsx
│   ├── 2_finalcompileddata.xlsx
│   └── 3_UP/
│   │   ├── 1_finalcompileddataup.csv
│   │   ├── 2_finalcompileddataup.xlsx
│   └── 4_WB/
│   │   ├── 1_finalcompileddatawb.csv
│   │   ├── 2_finalcompileddatawb.xlsx
└── README.md              # You are here!
````
---

## 🚀 Future Goals
- Extend framework to **other crops & regions**.  
- Integrate **real-time satellite and sensor data**.  
- Use **ARIMA models** for forecasting risks.  
- Compute **net premium** with risk loading + admin costs.  

---


