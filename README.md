# Final Project KKPM: Hypertension Classification

In this repository, we perform a comparative analysis of various classification algorithms with four different preprocessing techniques applied for hypertension classification.

Our objective was to explore and assess the impact of various data preprocessing strategies on the effectiveness and efficiency of machine learning models in addressing hypertension-related challenges.
## About Dataset
The hypertension dataset contains information related to patients and various factors that may influence the presence of hypertension (high blood pressure). 

### Data Source

The dataset was obtained from [https://www.kaggle.com/datasets/prosperchuks](https://www.kaggle.com/datasets/prosperchuks/health-dataset/?select=hypertension_data.csv).

### Data Description
This dataset consists of 14 attributes with 26.1k rows.
- **age**: patient's age (in years)
- **sex**: patient's gender (1: male; 0: female)
- **cp**: Chest pain type: 0: asymptomatic 1: typical angina 2: atypical angina 3: non-anginal pain
- **trestbps**: Resting blood pressure (in mm Hg)
- **chol**: Serum cholestoral in mg/dl
- **fbs**: if the patient's fasting blood sugar > 120 mg/dl (1: yes; 0: no)
- **restecg**: Resting ECG results: 0: normal 1: ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV) 2: probable or definite left ventricular hypertrophy by Estes' criteria
- **thalach**: Maximum heart rate achieved.
- **exang**: Exercise induced angina (1: yes; 0: no)
- **oldpeak**: ST depression induced by exercise relative to rest.
- **slope**: The slope of the peak exercise ST segment: 0: upsloping 1: flat 2: downsloping
- **ca**: Number of major vessels (0–3) colored by flourosopy
- **thal**: 3: Normal; 6: Fixed defect; 7: Reversable defect
- **target**: Whether the patient has hypertension (1) or not (0)

This dataset is valuable for exploring the relationships between various patient attributes and the likelihood of hypertension. It can be used for predictive modeling, classification tasks, and gaining insights into the factors contributing to high blood pressure in patients.
### Data Preprocessing

We implemented four preprocessing variations across five modeling algorithms, comprising the following types for each:

1. Baseline
2. Baseline with Normalization
3. Baseline with Normalization and Feature Selection
4. Baseline with Normalization, Feature Extraction, and Dimensional Reduction.

For details on these preprocessing steps, please refer to our repo.

## How to Use

These instructions will give you a copy of the project up and running on
your local machine for development and testing purposes. See deployment
for notes on deploying the project on a live system.

### Prerequisites

Requirements for the software and other tools to build, test and push 
- Python 3
- Git

### Installation

_Follow this step to run our code._

1. Clone the repo
   ```sh
   git clone https://github.com/saifudienrosyid/finalproject_KKPM.git
   ```
2. Create new Python virtual environment in the folder
   ```py
   python -m venv .venv 
   ```
3. Install dependencies to virtual environment
   ```py
   pip install -r requirements.txt
   ```
4. Set .venv as a kernel to execute the code.


## Evaluation Metrics

In this project, we use the following evaluation metrics for model assessment:

### Precision

Precision is calculated as the ratio of true positives to the sum of true positives and false positives:

$$ \text{Precision} = \frac{\text{True Positives}}{\text{True Positives + False Positives}} $$

### Recall (Sensitivity)

Recall measures the ability of the model to correctly identify all actual positive instances. It is calculated as the ratio of true positives to the sum of true positives and false negatives:

$$ \text{Recall} = \frac{\text{True Positives}}{\text{True Positives + False Negatives}} $$

### F1 Score

The F1 score is the harmonic mean of precision and recall, providing a balanced measure of model performance:

$$ \text{F1 Score} = \frac{2 \times \text{Precision} \times \text{Recall}}{\text{Precision + Recall}} $$

These metrics help us assess the model's performance in terms of precision, recall, and the overall balance between the two, which is critical for classification tasks.

## Results
Based on the evaluation metrics, we provide the classification performance results of 4 different preprocessing methods for 5 machine learning algorithms.

### 1. Baseline
|        | SVM         | GNB         | Ridge       | LDA         | LR          |
|--------|-------------|-------------|-------------|-------------|-------------|
| Prec   | 0.84 | 0.83 | 0.86 | 0.86 | 0.85 | 
| Rec    | 0.84 | 0.83 | 0.85 | 0.85 | 0.85 | 
| F1     | 0.84 | 0.83 | 0.85 | 0.85 | 0.85 | 
### 2. Baseline with Normalization
|        | SVM         | GNB         | Ridge       | LDA         | LR          |
|--------|-------------|-------------|-------------|-------------|-------------|
| Prec   | 0.84 | 0.83 | 0.86 | 0.86 | 0.85 | 
| Rec    | 0.84 | 0.83 | 0.85 | 0.85 | 0.85 | 
| F1     | 0.84 | 0.83 | 0.85 | 0.85 | 0.85 | 
### 3. Baseline with Normalization and Feature Selection
|        | SVM         | GNB         | Ridge       | LDA         | LR          |
|--------|-------------|-------------|-------------|-------------|-------------|
| Prec   | | | | | |
| Rec    | | | | | |
| F1     | | | | | |
### 4. Baseline with Normalization, Feature Extraction, and Dimensional Reduction.
|        | SVM         | GNB         | Ridge       | LDA         | LR          |
|--------|-------------|-------------|-------------|-------------|-------------|
| Prec   | | | | | |
| Rec    | | | | | |
| F1     | | | | | |


## Authors

  - **Mufti Alfarokhul Azam** - [Email](muftialfarokhulazam@mail.ugm.ac.id)
  - **Syaifudin Rosyid** -  [Email](saifudinrosyid@mail.ugm.ac.id)

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Acknowledgments

  - [prosperchuks](https://www.kaggle.com/prosperchuks) as the dataset provider
  - Inspiration