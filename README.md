# Air-Quality-Prediction-Using-Support-Vector-Regression
This project explores the use of Support Vector Regression (SVR) to estimate air pollutant concentrations using low-cost sensor data and environmental variables. The study focuses on understanding sensor behavior, data quality challenges, and the practical limitations of machine learning in real-world air quality monitoring systems.

Low-cost sensors provide indirect and noisy signals, while reference-grade instruments offer accurate but limited measurements. This project demonstrates how machine learning can act as a calibration bridge between these two systems.

Methodology

1. Data Cleaning & Preprocessing

Removed irrelevant and empty columns, Treated invalid sensor readings (-200) as missing values, Applied median imputation for skewed sensor and pollutant data, Standardized features for distance-based learning

2. Exploratory Data Analysis

Analyzed pollutant and sensor signal distributions, Identified skewness, noise, and variability patterns, Used insights to guide model selection and expectations

3. Machine Learning Modeling

Implemented Support Vector Regression (SVR) using scikit-learn, Compared Linear SVR vs RBF SVR, Used MAE, RMSE, and R² for evaluation, Trained separate models for each pollutant

4. Hyperparameter Tuning

Applied selective tuning for NOx(GT) due to high variability, Tuned a single parameter to demonstrate optimization capability, Observed modest improvements constrained by sensor noise

5. Visualization

Built Power BI dashboards using the cleaned dataset, Visualized pollutant distributions and sensor behavior, Used visuals to support and explain ML results

Key Findings

RBF SVR consistently outperformed Linear SVR

Benzene (C6H6) showed near-perfect predictability due to strong sensor alignment

CO and NO2 demonstrated moderate predictability

NOx was the most challenging pollutant due to chemical complexity and noise

Data quality and sensor sensitivity had greater impact than model complexity

Tools & Technologies

Python (Pandas, NumPy), Scikit-learn, Jupyter Notebook, Power BI
