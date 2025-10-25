
# Kenya NCD Risk Prediction Model

This project demonstrates a machine learning pipeline for predicting risk levels of non-communicable diseases (NCDs) using simulated health data inspired by Kenyan public health statistics.

## 📊 Dataset
- **File**: `kenya_ncd_simulated.csv`
- **Features**:
  - Age
  - BMI
  - Blood Pressure
  - Glucose Level
  - Smoker (0/1)
  - Alcohol Consumption (0/1)
  - Physical Activity (0–4 scale)
  - Family History (0/1)
  - Risk Level (0 = Low, 1 = Medium, 2 = High)

## 🧪 Pipeline Overview

### 1. Data Preprocessing
- Missing values are dropped.
- Features are scaled using `StandardScaler`.
- Data is split into training and test sets using stratified sampling.

### 2. Model Training
- A `RandomForestClassifier` is trained on the preprocessed data.
- The model is chosen for its robustness and interpretability.

### 3. Evaluation
- Accuracy and classification report are generated.
- `zero_division=0` is used to handle undefined precision due to class imbalance.

### 4. Visualization
- **Feature Importance**: Bar chart showing which features most influence predictions.
- **Risk Level Distribution**: Histogram showing the distribution of risk levels in the dataset.

## ⚖️ Ethical Considerations

### Bias
- Class imbalance may lead to poor prediction for high-risk individuals.
- Mitigation: Stratified sampling, synthetic data generation, and subgroup testing.

### Fairness
- Ensures equitable predictions across demographics.
- Mitigation: Use explainable AI and fairness audits.

### Sustainability
- Designed for low-resource environments.
- Mitigation: Efficient models, mobile-first design, and community engagement.

## 🚀 Usage
To run the model in Google Colab:
1. Upload `kenya_ncd_simulated.csv`.
2. Run the preprocessing, training, and visualization code.
3. Interpret results and explore ethical implications.

