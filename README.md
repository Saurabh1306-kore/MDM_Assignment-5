# Practical Assignment 5: Ensemble Learning and Performance Evaluation

## 1. Project Overview

This project is part of the TY B.Tech. Artificial Intelligence and Machine Learning practical assignment.

The main aim is to implement different ensemble learning techniques and compare their performance with individual machine learning models.

The project uses the **Breast Cancer Wisconsin Dataset** to classify tumors as malignant (cancerous) or benign (non-cancerous).

## 2. Objectives

1. Implement Stacking, AdaBoost and Voting Ensemble techniques.
2. Evaluate machine learning models using Accuracy, Precision, Recall and F1-score.
3. Compare ensemble models with individual machine learning models and identify the best-performing model.

## 3. Dataset

**Dataset Name:** Breast Cancer Wisconsin Diagnostic Dataset

**Source:** Scikit-learn (`load_breast_cancer`)

The dataset contains:

- 569 samples
- 30 input features
- 2 target classes: Malignant (0) and Benign (1)

The dataset is divided into:

- Training data: 80%
- Testing data: 20%

StandardScaler is used for feature scaling where required.

## 4. Machine Learning Models Implemented

### Individual ML Models

1. **Logistic Regression:** A classification algorithm that predicts the probability of a class.
2. **Decision Tree:** A model that makes predictions using decision rules.
3. **K-Nearest Neighbors (KNN):** A model that classifies data based on nearby samples.

### Ensemble Learning Models

1. **Stacking Ensemble:** Combines Logistic Regression, Decision Tree and KNN using Logistic Regression as a meta-classifier.
2. **AdaBoost Ensemble:** Combines 50 weak Decision Tree classifiers (decision stumps) to improve classification.
3. **Hard Voting Ensemble:** Combines Logistic Regression, Decision Tree and KNN using majority voting.

## 5. Technologies and Libraries Used

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## 6. Implementation Steps

1. Import the required Python libraries.
2. Load the Breast Cancer Wisconsin Dataset.
3. Check dataset information and missing values.
4. Separate input features and target labels.
5. Split the dataset into training and testing data.
6. Apply feature scaling where required.
7. Train Logistic Regression, Decision Tree and KNN.
8. Implement and train Stacking Ensemble.
9. Implement and train AdaBoost Ensemble.
10. Implement and train Hard Voting Ensemble.
11. Predict the test data using all six models.
12. Calculate Accuracy, Precision, Recall and F1-score.
13. Compare the models using tables and graphs.
14. Generate confusion matrices and analyze incorrect predictions.
15. Save the final performance comparison as a CSV file.

## 7. Model Performance Comparison

The following results were obtained from the Google Colab experiment.

| Model | Accuracy | Precision | Recall | F1-score |
|---|---|---|---|---|
| Logistic Regression | 0.9825 | 0.9812 | 0.9812 | 0.9812 |
| Decision Tree | 0.9123 | 0.9019 | 0.9157 | 0.9075 |
| KNN | 0.9561 | 0.9551 | 0.9504 | 0.9526 |
| Stacking | 0.9825 | 0.9865 | 0.9762 | 0.9810 |
| AdaBoost | 0.9561 | 0.9605 | 0.9454 | 0.9521 |
| Voting | 0.9825 | 0.9865 | 0.9762 | 0.9810 |

Precision, Recall and F1-score are calculated using macro averaging.

## 8. Results and Observations

- **Best Overall Model:** Logistic Regression, with the highest macro F1-score of 0.9812.
- **Best Ensemble Models:** Stacking and Voting, both achieving 98.25% accuracy and 0.9810 macro F1-score.
- AdaBoost performed better than the individual Decision Tree.
- Decision Tree achieved the lowest accuracy of 91.23%.
- Ensemble models did not outperform Logistic Regression in this experiment.

## 9. Graphs and Visualizations

The Google Colab notebook includes:

1. Accuracy comparison of all six models.
2. Comparison of Accuracy, Precision, Recall and F1-score.
3. Confusion matrices for all six models.

These graphs help us understand the performance differences between individual and ensemble models.

## 10. How to Run the Project

1. Download the `AIML_Assignment_5_Ensemble_Learning.ipynb` notebook from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload the notebook.
4. Run all cells in sequence.
5. View the model outputs, performance tables and graphs.
6. Download the generated `ensemble_model_comparison.csv` file if required.

The dataset is loaded directly from Scikit-learn, so no separate dataset download is required.

## 11. Conclusion

In this practical, three individual machine learning models and three ensemble learning models were implemented and evaluated.

Logistic Regression achieved the highest macro F1-score, while Stacking and Voting achieved the best performance among ensemble methods.

This practical helped me understand ensemble learning, model training, classification metrics and performance comparison.

## 12. Future Improvements

- Apply hyperparameter tuning to improve model performance.
- Use repeated cross-validation for more reliable evaluation.
- Test the models on additional classification datasets.
- Improve the detection of malignant cases by analyzing class-specific recall.

## 13. Limitations and Ethical Considerations

The models were evaluated using one dataset and one train-test split, so their performance may vary on other datasets.

Since the project involves breast cancer classification, identifying malignant cases correctly is important. These models are developed for educational purposes and should not be used for real medical diagnosis without proper clinical validation.

## 14. Student Details

**Student Name:** Saurabh Dharma Kore  
**PRN:** 202401070159  
**Branch:** Electronics and Telecommunication Engineering (ENTC)  
**College:** MIT Academy of Engineering, Alandi, Pune  
**Practical No.:** 5  
**Subject:** Artificial Intelligence and Machine Learning

---

**Project Type:** Academic Practical Assignment  
**Language:** Python  
**Platform:** Google Colab
