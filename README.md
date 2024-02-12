## Feature: Multi-Algorithm Activity Recognition

### Description:
The Human Activity Recognition System incorporates a multi-algorithm approach to enhance the accuracy and adaptability of activity classification.

### Key Components:
1. **Support Vector Classifier (SVC):**
   - Utilizes support vector machines to classify activities based on the learned patterns from the training dataset.

2. **K Nearest Neighbor (KNN):**
   - Employs the k-nearest neighbor algorithm to classify activities by comparing the feature vectors of test instances with the ones in the training dataset.

3. **Logistic Regression:**
   - Implements logistic regression for binary classification tasks, providing a probabilistic framework for activity recognition.

4. **Random Forest:**
   - Leverages an ensemble of decision trees to enhance accuracy and robustness in classifying complex activity patterns.

### Advantages:
- **Diversity in Modeling:**
  - Each algorithm brings a unique perspective to activity recognition, allowing the system to adapt to different types of datasets and scenarios.

- **Comprehensive Performance Evaluation:**
  - Enables users to compare and contrast the effectiveness of each algorithm through thorough evaluation metrics.

- **Flexible Integration:**
  - The modular design facilitates the addition of new algorithms or the removal of existing ones, providing flexibility for future enhancements.

### Dataset:
The dataset used for training and evaluating the models can be found [here](https://www.kaggle.com/code/fahadmehfoooz/human-activity-recognition-with-neural-networks/input).

### Usage:
To utilize the multi-algorithm activity recognition feature, follow these steps:
1. Load the dataset.
2. Choose the desired algorithm(s) for training and recognition.
3. Train the model using the provided scripts or API.
4. Evaluate the model's performance with the included evaluation metrics.
5. Integrate the recognized activity labels into your application or analysis.

### Examples:
```python
# Example code snippet for using SVC
from sklearn.svm import SVC

# Instantiate the SVC model
svc_model = SVC()

# Train the model
svc_model.fit(X_train, y_train)

# Predict activities
predictions_svc = svc_model.predict(X_test)
