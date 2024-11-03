# Linear Regression Health Costs Calculator 💊

## Project Overview
This project aims to predict healthcare costs using a linear regression model. Given a dataset containing demographic information and healthcare expenses for various individuals, the model will be trained to forecast costs based on new input data.

## Challenge Description
In this challenge, you will develop a regression model to predict healthcare expenses. The project involves data preprocessing, model training, and evaluation to ensure the model predicts costs accurately.

## Dataset
You will be working with a dataset that includes:
- Demographic information of individuals (e.g., age, sex, BMI, etc.)
- Corresponding healthcare costs.

### Data Preprocessing
1. **Import Libraries and Data**: The first two cells in the notebook will handle this.
2. **Convert Categorical Data**: Convert any categorical variables to numeric format to facilitate model training.
3. **Split the Data**:
   - Use **80%** of the data for training (`train_dataset`).
   - Use **20%** of the data for testing (`test_dataset`).

4. **Create Labels**: Remove the `expenses` column from both datasets to form `train_labels` and `test_labels` for training the model.

## Model Training and Evaluation
1. **Train the Model**: Utilize the training dataset to fit your regression model.
2. **Evaluate the Model**: The final cell of the notebook will evaluate the model using the test dataset. Ensure that `model.evaluate` returns a Mean Absolute Error (MAE) of under **3500**, indicating accurate predictions of healthcare costs.

### Example Evaluation Code
```python
# Evaluate the model
mae = model.evaluate(test_dataset, test_labels)
print("Mean Absolute Error:", mae)
