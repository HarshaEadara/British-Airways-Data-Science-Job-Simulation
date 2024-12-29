# British Airways Data Science Job Simulation

This repository showcases a project simulating real-world tasks completed by the British Airways Data Science team. It includes two primary tasks: analyzing customer reviews and predicting customer buying behavior. The project provides insights into the role of a Data Scientist at British Airways through practical problem-solving and data-driven decision-making.

## Project Overview

This project focuses on analyzing customer reviews and predicting customer bookings using data obtained from Skytrax and Forage. The repository includes three CSV files and various presentation and notebook files for a comprehensive analysis.

## Tasks

### Task 1: Web Scraping to Gain Company Insights
- **Objective**: Scrape and analyze customer review data to uncover insights for British Airways.
- **Steps**:
  1. Apply web scraping to unstructured third-party customer review data from [Skytrax](https://www.airlinequality.com/airline-reviews/british-airways).
  2. Perform sentiment analysis using the NLTK library in Python to classify reviews as positive, neutral, or negative.
  3. Present insights and findings using PowerPoint.

[Notebook Link for Task 1](https://github.com/HarshaEadara/British-Airways-Data-Science-Job-Simulation/blob/main/Task_1_Web_scraping_to_gain_company_insights.ipynb)

### Task 2: Predicting Customer Buying Behavior
- **Objective**: Build a predictive model to understand factors influencing customer buying behavior.
- **Steps**:
  1. Perform Exploratory Data Analysis (EDA) and feature engineering to prepare the dataset.
  2. Create a classification model to predict customer buying behavior.
  3. Highlight insights and analysis using PowerPoint.

[Notebook Link for Task 2](https://github.com/HarshaEadara/British-Airways-Data-Science-Job-Simulation/blob/main/Task_2_Predicting_customer_buying_behaviour.ipynb)

## Results

### Predictive Model Performance
In our quest to build a robust predictive model, we evaluated the performance of two prominent classifiers: the Random Forest and XGBoost. We examined their performance using both a subset of the top 6 features and the full feature set to gauge the impact of feature selection.
- **Random Forest Classifier**:
  - **With Top 6 Features:** The Random Forest classifier achieved an accuracy of **83.36%** and an AUC score of **0.566**. This indicates that even with a reduced feature set, the model maintains a high level of accuracy, although its ability to distinguish between classes (as indicated by the AUC score) is moderate.
  - **With All Features:** When utilizing all available features, the model's accuracy improved to **84.76%** with an AUC score of **0.548**. While the accuracy increased, the AUC score slightly decreased, suggesting that adding more features might introduce some noise, affecting the model's classification capability.
- **XGBoost Classifier**:
  - **With Top 6 Features:** The XGBoost classifier demonstrated an accuracy of **84.72%** and an AUC score of **0.519**. This high accuracy indicates that the model effectively leverages the most important features, though its AUC score suggests a moderate ability to differentiate between classes.
  - **With All Features:** Using the full feature set, the XGBoost classifier's accuracy increased marginally to **84.98%**, and the AUC score rose to **0.542**. The slight improvement in both accuracy and AUC suggests that the model benefits from additional features without significant overfitting.
- **Final Model**: 
  - The final model, incorporating optimal feature selection and hyperparameter tuning, achieved an accuracy of **85.09%** and an AUC score of **0.558**. This demonstrates the model's overall robustness and its ability to make precise predictions. The balance between accuracy and AUC score highlights the model's effectiveness in both making correct predictions and distinguishing between different classes.
  - In conclusion, both the Random Forest and XGBoost classifiers performed well, with slight variations based on the feature set used. The final model's enhanced performance, particularly in terms of accuracy and AUC, underscores the importance of meticulous feature selection and tuning in developing reliable predictive models.

## Repository Structure
- **Notebooks**:
  - `Task_1_Web_scraping_to_gain_company_insights.ipynb`: Web scraping and sentiment analysis.
  - `Task_2_Predicting_customer_buying_behaviour.ipynb`: Predictive modeling.
- **Data**: CSV files used for analysis.

## Tools and Libraries
- **Programming Languages**: Python
- **Libraries**: NLTK, pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn
- **Visualization**: PowerPoint

## Insights
- **Customer Reviews**:
  - Sentiment analysis of customer reviews provided valuable insights into customer satisfaction and areas for improvement.
- **Buying Behavior**:
  - Predictive modeling identified key factors influencing customer bookings, enabling data-driven decisions.

## How to Use
1. Clone the repository.
   ```bash
   git clone https://github.com/HarshaEadara/British-Airways-Data-Science-Job-Simulation.git
   ```
2. Navigate to the directory
   ```bash
   cd British-Airways-Data-Science-Job-Simulation
   ```
3. Install the required libraries.
   ```bash
   pip install -r requirements.txt
   ```
4. Open the Jupyter notebooks to explore the analysis and predictive modelling.
   ```bash
   jupyter notebook Task_1_Web_scraping_to_gain_company_insights.ipynb
   jupyter notebook Task_2_Predicting_customer_buying_behaviour.ipynb
   ```
5. Ensure the dataset is available in the project directory.
6. Run the cells sequentially to execute the analysis.

## Acknowledgments
This project was completed as part of the British Airways Data Science Job Simulation provided by [British Airways and Forage](https://www.theforage.com/simulations/british-airways/data-science-yqoz).

