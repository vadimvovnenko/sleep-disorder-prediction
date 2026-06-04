# Sleep Disorder Prediction

ML project predicting sleep disorders (Insomnia / Sleep Apnea / None) 
based on lifestyle and physiological features.

## Dataset
- 374 individuals
- 12 features: age, BMI, stress level, sleep duration, occupation, etc.
- Target: Sleep Disorder (None / Insomnia / Sleep Apnea)

## Methods
- Exploratory Data Analysis (EDA)
- Data preprocessing: LabelEncoder, feature engineering
- Class imbalance handling: SMOTE
- Models: Random Forest, XGBoost

## Results

| Model | Accuracy |
|---|---|
| Random Forest + SMOTE | 79% |
| XGBoost + SMOTE | 80% |

Best recall on minority classes achieved with XGBoost + SMOTE.  
Most important feature: **BMI Category** (linked to Sleep Apnea).

## Limitations
- Small dataset (n=374) — minority classes underrepresented
- SMOTE generates synthetic data, not real clinical cases
- Real PSG/EEG data would significantly improve results

## Tech Stack
Python, pandas, scikit-learn, XGBoost, imbalanced-learn, matplotlib, seaborn
