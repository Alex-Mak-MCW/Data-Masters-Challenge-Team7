#  Energy Usage Forecast with Data Science & Machine Learning

## 📚 Table of Contents

- [Project Overview](#project-overview)
- [The Problem](#the-problem)
- [Our Mission](#our-mission)
- [Data-Driven Deliverables](#data-driven-deliverables)
- [Tech Stack](#tech-stack)
- [How to Use This Repository](#how-to-use-this-repository)
- [Overall Findings](#overall-findings)
- [Acknowledgements](#acknowledgements)

## Project Overview

Our team participated in the 3-Day Data Masters Challenge Olympiad (April 25–27, 2025), co-hosted by the University of Alberta's Modeling, Data, and Predictions (MDP) Program and Canisius University's Canisius Center for Analytics and Data Ecosystems (CCADE). 

We tackled a real-world challenge in energy optimization for a large real estate investment trust (REIT) and are proud to share that we placed **3rd overall** in the competition!

### The Problem:
The REIT manages over 1,600 commercial buildings across North America and Europe is facing surging energy costs, carbon emission penalties, and significant inefficiencies in energy usage. Hence they would like to achieve the following objective:

🎯 **Reduce energy waste by 20% within two years without compromising building functionality** 🎯

### Our Mission

Our goal was to determine whether the REIT's energy efficiency target is achievable and, if so, how successfully it can be met using data-driven approaches.

We conducted four key phases:

1. **Data Cleaning & Preparation**
   - Applied **data cleaning** techniques such as linear interpolation, Last Observation Carried Forward (LOCF), and Next Observation Carried Backward (NOCB) to handle missing data.
   - Performed **anomaly detection** using z-score analysis to flag outliers and unexpected meter readings.

2. **Exploratory Data Analysis (EDA)**
   - Identified high-consumption buildings as candidates for targeted energy interventions.
   - Detected inefficiencies including unusual weekend activity and usage spikes.
   - Analyzed seasonal and operational trends influencing energy demand.

3. **Predictive Modeling**
   - Developed, tuned, and evaluated state-of-the-art deep learning models including Long-Short Term Memory (LSTM) and Gated Recurrent Units (GRU) to forecast future energy consumption.
   - Achieved up to **85% overall forecasting accuracy**, and **90%+** on more than half of the building types.

4. **Actionable Recommendations**
   - Investigate anomalies and fix missing data.
   - Introduce proactive resource management based on usage trends.
   - Audit inefficient buildings and explore alternative energy sources.

## Data-Driven Deliverables

📂 This repository includes:

- 📄 [Data Cleaning & EDA Notebook](./Python_Notebooks/Preprocessing_and_EDA.ipynb)
- 📄 [LSTM Model – by Location Notebook](./Python_Notebooks/LSTM_by_Location.ipynb)
- 📄 [LSTM Model – by Usage Notebook](./Python_Notebooks/LSTM_by_Use.ipynb)
- 📄 [GRU Model Notebook](./Python_Notebooks/GRU_by_use.ipynb)

📌 We also prepared two written reports (not included here):
  - A technical report illustrating the entire data preprocessing and EDA pipeline
  - A business consulting report based on the findings we derived from our EDA and predictive modeling work.
    
  **Please contact us if you are interested in knowing more about them!**

## Tech Stack

🤖 **ML/Modeling**: TensorFlow, Keras, Scikit-learn  
📊 **EDA & Processing**: Pandas, NumPy, Scipy, Statsmodels, Matplotlib, Seaborn  
🛠️ **Environment**: Jupyter Notebook, GitHub


## How to Use This Repository

1. Clone or download the repository:
   ```bash
   git clone https://github.com/Alex-Mak-MCW/Data-Masters-Challenge-Team7.git
   ```
2. Unzip the cleaned data from the data folder 
3. Run the Python Notebook files you wish to try!

## Overall Findings

Our analysis and modeling produced the following key findings and takeaways:

💡  Identified **22 anomalies** out of 17,522 time entries (≈0.13%), recommending further investigation to prevent long-term energy and cost waste.

💡 Found that **8.92% of all readings were missing**, indicating the need to repair or recalibrate faulty meters to enhance future forecasting and reduce inefficiencies.

💡 Discovered a clear **24-hour usage pattern**: energy use peaks during working hours (9 a.m. – 6 p.m.) and drops significantly overnight (12 a.m. – 6 a.m.), with a **25% consumption gap**.

💡 Detected **seasonal variation**: summer months (June–September) showed a **12.5% increase** in consumption compared to the rest of the year.

💡 Achieved **85% overall forecasting accuracy**, with **over 90% on most building types**, validating the strength of our LSTM and GRU models.

💡 Demonstrated that our model can enable **proactive energy management** through strategies like **load shifting** and **demand response**, supporting optimized infrastructure planning.

Altogether, if our client implements the proposed recommendations and adopts our forecasting model (with 90%+ accuracy for most building types), we estimate they can limit energy waste to **10% or less**, with potential for further reduction depending on implementation success.

## Acknowledgements 
We would like to thank the University of Alberta's MDP Program and all the organizers of the Data Masters Challenge Olympiad for the opportunity to apply our skills in a real-world context. It was a rewarding experience in both data science and team collaboration!
