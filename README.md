# 🏏 IPL Live Match Win Probability Engine (2008 - 2025)

An end-to-end predictive analytics application designed to calculate real-time chasing probabilities during the second innings of an Indian Premier League (IPL) match. Leveraging historical ball-by-ball data spanning from 2008 through the 2025 season, this repository transitions raw sports statistics into a production-ready machine learning asset integrated with an interactive web dashboard.

## 🚀 Key Features

* **Advanced Feature Engineering:** Computes live, rolling game state variables dynamically, including Runs Remaining, Balls Remaining, Wickets Left, Current Run Rate (CRR), and Required Run Rate (RRR).
* **Robust Preprocessing Pipeline:** Systematically handles historical franchise rebrands (e.g., standardizing *Delhi Daredevils* to *Delhi Capitals* and *Kings XI Punjab* to *Punjab Kings*) and filters out anomalies to ensure data consistency.
* **Seamless Pipeline Serialization:** Utilizes Scikit-Learn `Pipeline` and `ColumnTransformer` arrays to bundle categorical One-Hot Encoding rules tightly with a calibrated `LogisticRegression` classifier, preventing data leakage during live inference.
* **Production Deployment:** Embedded within an interactive **Streamlit UI** featuring an optimized slider component (`format="%g"`) to cleanly display precise cricket over intervals (e.g., `8.5`, `14.3`) without floating-point padding defects.

## 🛠️ Tech Stack & Architecture

* **Language:** Python
* **Data Engineering & Analytics:** Pandas, NumPy
* **Machine Learning Framework:** Scikit-Learn (Logistic Regression, Train-Test Split, ColumnTransformer, ML Pipelines)
* **Model Serialization:** Pickle
* **User Interface Framework:** Streamlit Cloud Dashboard
