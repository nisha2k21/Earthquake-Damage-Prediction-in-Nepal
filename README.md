# Earthquake Damage Prediction in Nepal

## Overview

This project focuses on predicting the severity of building damage caused by the 2015 Gorkha Earthquake in Nepal. Using data from Open Data Nepal, the project aims to build machine learning models that can classify the extent of building damage, aiding in disaster response and planning. The goal is to create a tool that can help local authorities and organizations quickly assess and prioritize areas for rebuilding efforts.

## Project Highlights
- **Objective**: Predict the severity of building damage using historical earthquake data.
- **Data Source**: [Open Data Nepal](https://data.opennepal.net/), which provides detailed information on the Gorkha Earthquake and its impact on infrastructure.
- **Tools Used**: Python, SQL, Pandas, scikit-learn, matplotlib, and seaborn.
- **Techniques**: Logistic regression, decision trees, data resampling, and model evaluation using classification metrics.

## Workflow
1. **Data Collection**: 
   - Downloaded earthquake impact data from Open Data Nepal, focusing on building damage severity.
   - Queried a SQL database to extract relevant features such as building types, materials used, and geographic location.

2. **Data Preprocessing**:
   - Cleaned and processed the data using Pandas, addressing missing values and correcting any inconsistencies.
   - Handled imbalanced data by applying resampling techniques such as oversampling and undersampling.
   - Performed exploratory data analysis (EDA) to understand key features and their correlations with damage severity.

3. **Modeling**:
   - Built multiple classification models, including **logistic regression** and **decision tree classifiers**, to predict damage severity.
   - Fine-tuned hyperparameters using grid search and cross-validation to improve model performance.
   - Evaluated models using classification metrics such as accuracy, precision, recall, and F1-score.

4. **Prediction**:
   - Used the best-performing model to classify buildings into different damage categories based on input features.
   - Visualized the prediction results to help authorities understand the impact distribution and focus disaster response accordingly.

## Results
- The **decision tree model** outperformed logistic regression in predicting severe damage cases, especially in imbalanced data scenarios.
- The model achieved high precision and recall, accurately identifying critical areas that require immediate attention for rebuilding and disaster relief.

## Key Learnings
- **SQL Querying**: Learned to efficiently query and manipulate data stored in SQL databases for analysis.
- **Machine Learning**: Gained hands-on experience in building, tuning, and evaluating classification models for real-world disaster scenarios.
- **Data Resampling**: Successfully handled imbalanced data using resampling techniques to ensure that minority classes (severe damage) were adequately represented.
  
## Future Improvements
- **Incorporate Geospatial Data**: Integrate geospatial features such as proximity to fault lines or elevation data to improve prediction accuracy.
- **Advanced Models**: Experiment with ensemble models like Random Forest or Gradient Boosting to enhance model performance.
- **Deployment**: Develop a web-based tool or dashboard to allow easy input of new data and real-time damage prediction after future earthquakes.

## Installation and Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/nisha2k21/earthquake-damage-nepal.git
   ```
   
2. Navigate to the project directory:
   ```bash
   cd earthquake-damage-nepal
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the model to make predictions:
   ```bash
   python src/damage_prediction.py
   ```

## Project Structure
```
├── data
│   └── earthquake_damage_data.csv   # Raw data file
├── notebooks
│   └── EDA_and_Modeling.ipynb       # Jupyter notebook for analysis and model building
├── src
│   └── damage_prediction.py         # Python script for running the model
├── requirements.txt                 # List of required dependencies
└── README.md                        # Project documentation
```

## Technologies Used
- **Programming Language**: Python
- **Database**: SQL
- **Libraries**: Pandas, NumPy, scikit-learn, matplotlib, seaborn
- **Machine Learning**: Logistic regression, Decision tree classifiers
- **Model Evaluation**: Precision, Recall, F1-score, Accuracy

## Contact
For any questions or collaboration opportunities, feel free to reach out:
- **Email**: nisha2k21@gmail.com
- **LinkedIn**: [Nisha Kumari](https://www.linkedin.com/in/nisha-kumari-041300225/)

---

This README file covers all the essential aspects of your project, including its objectives, workflow, results, and potential future improvements. It’s structured to provide a clear overview for both collaborators and recruiters interested in your work.
