# Hear-Attack-Analysis

This project is focused on heart attack prediction using machine learning. Here's a comprehensive breakdown of the project:

Main Objective:
- Building a machine learning model to predict the risk of heart attacks based on patients' health conditions using various medical features

Dataset Overview:


1. Demographic data:
   - Age (in years)
   - Gender (0 = female, 1 = male)

2. Clinical measurements:
   - Blood pressure (trtbps)
   - Cholesterol levels (chol)
   - Fasting blood sugar (fbs)
   - Maximum heart rate (thalachh)

3. Test results:
   - Chest pain type (cp)
   - Resting ECG results (restecg)
   - Exercise-induced angina (exng)
   - ST depression (oldpeak)
   - ST segment slope (slp)
   - Number of major vessels (caa)
   - Thallium stress test results (thall)

Key Analysis Steps:
1. Data Cleaning:
   - Removed duplicate entries
   - Checked for null values
   - Reset indices

2. Exploratory Data Analysis:
   - Created visualizations for feature distributions
   - Analyzed correlations between features
   - Found that features like chest pain, maximum heart rate, and ST slope were highly correlated with heart attack risk

3. Data Preprocessing:
   - Applied feature scaling using StandardScaler and MinMaxScaler
   - Split data into training (80%) and testing (20%) sets

4. Model Implementation:
   - Logistic Regression:
     * Achieved 82% accuracy
     * Good balance between precision and recall

   - Decision Tree:
     * Tested various depths (1-49)
     * Achieved consistent accuracy around 82%

   - Random Forest:
     * Best performing model with 88.5% accuracy
     * Showed excellent precision (95% for negative class, 85% for positive class)
     * High recall for positive cases (97%)

The project includes functionality to make predictions on new patient data, providing both the prediction (higher/lesser chance of heart attack) and probability scores.

Key Findings:
1. Majority of patients were over 40 years old
2. Dataset had twice as many males as females
3. About 54.3% of patients had a high chance of heart attack
4. Normal test results generally indicated lower heart attack risk
5. The most influential factors were chest pain, maximum heart rate, exercise-induced angina, ST depression, and number of major vessels

This project provides a practical tool for initial heart attack risk assessment, though it should be used in conjunction with professional medical advice.
