# Iris Classification using Random Forest

## Objective:

The objective of this project is to develop a machine learning model that classifies different species of Iris flowers based on their features: sepal length, sepal width, petal length, and petal width. The model is built using a Random Forest Classifier and evaluated based on accuracy, classification report, and confusion matrix.

## Approach:

1. **Data Loading and Preprocessing**:

   - The Iris dataset is loaded from a CSV file (`IRIS.csv`).
   - The target variable (`species`) is encoded using `LabelEncoder` to convert categorical labels into numerical values.
   - The features are scaled using `StandardScaler` to normalize the values, improving model performance.

2. **Model Training**:

   - A Random Forest Classifier is trained on the dataset with a train-test split (80% training, 20% testing).
   - Hyperparameters of the model are kept simple and can be tuned for further improvement.

3. **Evaluation**:

   - The model's performance is evaluated using accuracy, a classification report, and a confusion matrix.
   - The confusion matrix is visualized using a heatmap for better understanding of classification errors.

4. **Model Saving**:
   - The trained Random Forest model, feature scaler, and label encoder are saved using `joblib` to enable future use in predictions without retraining.

## Challenges Faced:

- **Class Imbalance**: The dataset has a balanced distribution of target classes, but challenges might arise in real-world applications with imbalanced datasets.
- **Data Preprocessing**: Ensuring that preprocessing steps like scaling and encoding are applied consistently during both training and prediction.

## Results:

- **Accuracy**: The model achieved an accuracy of **97.8%** on the test set.
- The model performed well in classifying Iris species based on the four features provided.
