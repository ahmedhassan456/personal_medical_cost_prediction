
# Personal Medical Cost Prediction

This project uses a **RandomForestRegressor** model to predict individual medical costs billed by health insurance companies based on various factors such as age, gender, BMI, number of children, smoking status, and region of residence. 

## Dataset

The dataset used in this project is sourced from the book *Machine Learning with R* by Brett Lantz. The dataset was cleaned and recoded to match the format in the book. Below are the details of the dataset:

### Columns:

- **age**: Age of the primary beneficiary.
- **sex**: Insurance contractor's gender (female, male).
- **bmi**: Body mass index, an objective index of body weight (kg/m^2) using the ratio of height to weight. Ideally ranges from 18.5 to 24.9.
- **children**: Number of children covered by health insurance or the number of dependents.
- **smoker**: Smoking status (yes/no).
- **region**: The beneficiary's residential area in the US (northeast, southeast, southwest, northwest).
- **charges**: Individual medical costs billed by health insurance.

## Project Overview

### Goal
The goal of this project is to predict the `charges` column, which represents the individual medical costs billed by health insurance companies.

### Model Used
- **RandomForestRegressor**: A machine learning model that builds multiple decision trees and merges them together to get a more accurate and stable prediction.

### Process

1. **Data Exploration and Preprocessing**
   - Analyzed the distribution of features.
   - Checked for missing values and performed necessary cleaning.
   - Encoded categorical variables.
   - Split the dataset into training and testing sets.

2. **Model Training**
   - Trained a RandomForestRegressor model using the training dataset.
   - Performed hyperparameter tuning to improve model performance.

3. **Model Evaluation**
   - Evaluated the model using metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared score.
   - Visualized the results and interpreted the model's predictions.

### Results
The model was able to predict medical costs with reasonable accuracy, capturing the influence of various factors like BMI, smoking status, and age on the medical costs.

## Repository Structure

- `personal_medical_cost_prediction.ipynb`: The Jupyter Notebook containing the code, analysis, and visualizations.
- `data/`: The dataset used for the project (if applicable).
- `README.md`: This file.

## Requirements

- Python 3.x
- Libraries: 
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

## How to Run the Project

1. Clone this repository.
2. Ensure you have the required libraries installed by running `pip install -r requirements.txt`.
3. Open the `personal_medical_cost_prediction.ipynb` notebook.
4. Run the cells in the notebook to see the data exploration, model training, and evaluation process.

## Conclusion

This project demonstrates the application of a RandomForestRegressor to predict personal medical costs. The model achieved a good balance between bias and variance, making it a reliable tool for estimating medical expenses based on the given features.

## Acknowledgements

- Dataset: *Machine Learning with R* by Brett Lantz.
