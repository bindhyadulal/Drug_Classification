# Drug Type Prediction

This project uses machine learning techniques to predict the type of drug a patient is likely to be prescribed based on features such as gender, blood pressure, and cholesterol levels. The dataset used in this project is `drug200.csv`, which contains information about patients and the drugs they were prescribed.

## Requirements

- Python 3.x
- Libraries: `matplotlib`, `seaborn`, `pandas`, `numpy`, `sklearn`

Install the required libraries using `pip`:
```bash
pip install matplotlib seaborn pandas numpy scikit-learn
```

## Dataset Overview

The dataset consists of the following features:

- **Sex**: Gender of the patient (Male/Female)
- **BP**: Blood pressure levels (Low/Normal)
- **Cholesterol**: Cholesterol levels (Normal/High)
- **Na_to_K**: Sodium to Potassium ratio
- **Drug**: Drug prescribed to the patient (target variable)

## Steps Involved in the Project

### 1. **Data Preprocessing**:
   - The dataset is cleaned and prepared for analysis.
   - Categorical variables (e.g., `Sex`, `BP`, `Cholesterol`, `Drug`) are encoded using one-hot encoding or label encoding.
   - Missing values and duplicates are handled, and the first column (index) is dropped.

### 2. **Data Visualization**:
   - Various visualizations are used to understand the distribution of features and the relationships between them:
     - Drug type distribution
     - Gender distribution
     - Blood pressure distribution
     - Cholesterol distribution
     - Gender distribution based on drug type
     - Blood pressure distribution based on cholesterol

   These visualizations help in understanding the correlation between different features and the target variable.

### 3. **Feature Engineering**:
   - One-hot encoding is used to convert categorical variables into binary format.
   - The dataset is split into training and testing sets using `train_test_split`.

### 4. **Model Building**:
   Several machine learning models are trained and evaluated:
   - **Logistic Regression**
   - **Decision Tree Classifier**
   - **Random Forest Classifier**
   
   These models are evaluated using metrics such as accuracy, classification report, confusion matrix, and heatmaps for visualizing the model performance.

### 5. **Model Evaluation**:
   After training the models, they are evaluated based on their performance on the test dataset. The performance of the models is compared, and the best performing model is selected based on accuracy.

### 6. **Model Comparison**:
   A summary table is created to compare the accuracy of different models.

## Steps to Run the Project

1. **Download the Dataset**: Make sure you have the `drug200.csv` dataset. Ensure it is in the correct path relative to your script.

2. **Run the Script**:
   - Ensure you have all the dependencies installed.
   - Run the Python script to execute the data preprocessing, visualization, model building, and evaluation.

   The script will display various plots showing data distributions and model performances, including confusion matrices.

3. **Output**:
   - You will see accuracy values and classification reports for each model.
   - Confusion matrices will be displayed for each model's performance.
   - A comparison table of all models' accuracies will be shown.

## Example Output

```text
Logistic Regression accuracy is: 84.00%
Decision Tree Accuracy is: 85.00%
Random Forest accuracy is: 87.00%
```

- The comparison table will show which model performed best in predicting the drug type based on the features.

## License

This project is open-source and free to use. You can modify and distribute it under the terms of the MIT License.
