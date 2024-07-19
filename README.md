# Support Vector Machines Project

This project demonstrates the use of Support Vector Machines (SVM) for classification using the famous [Iris flower data set](http://en.wikipedia.org/wiki/Iris_flower_data_set).

## Overview

The Iris flower data set, also known as Fisher's Iris data set, is a multivariate data set introduced by Sir Ronald Fisher in 1936 as an example of discriminant analysis. It consists of 150 samples from three species of Iris flowers (Iris setosa, Iris virginica, and Iris versicolor). Each sample includes four features: sepal length, sepal width, petal length, and petal width, all measured in centimeters.

### Iris Data Set Details

- **Number of Samples:** 150
- **Number of Species:** 3 (Iris setosa, Iris versicolor, Iris virginica)
- **Number of Features:** 4 (sepal length, sepal width, petal length, petal width)

## Project Workflow

1. **Loading the Dataset:**
   - The Iris dataset is loaded using appropriate libraries.

2. **Exploratory Data Analysis (EDA):**
   - A pairplot of the dataset is plotted to visualize the distribution and relationships between features.
   - A Kernel Density Estimate (KDE) plot of `sepal_length` vs. `sepal_width` is created specifically for the Iris setosa species.

3. **Data Splitting:**
   - The dataset is split into training and testing sets using `train_test_split`.

4. **Model Training and Evaluation:**
   - An SVM model is instantiated using `SVC`.
   - The model is fitted to the training data.
   - Predictions are made on the test data.
   - The accuracy of the model is evaluated and found to be quite good.

5. **Hyperparameter Tuning with GridSearch:**
   - A dictionary of grid parameters is created for hyperparameter tuning.
   - A `GridSearchCV` object is instantiated and fitted to the training data.
   - The best parameters and the best estimator are obtained.
   - Predictions are made using the tuned model.
   - The tuned model's performance is evaluated. The confusion matrix indicates one noisy point that was not predicted correctly, but this is acceptable to avoid overfitting.

## Files in the Repository

- `Support Vector Machines Project.ipynb`: The Jupyter Notebook containing the complete code and analysis.

## How to Run

1. Clone the repository.
2. Ensure you have the necessary dependencies installed (e.g., `scikit-learn`, `seaborn`, `matplotlib`, `pandas`).
3. Open the Jupyter Notebook `Support Vector Machines Project.ipynb`.
4. Run the cells in the notebook to see the analysis and results.

## Conclusion

This project showcases the application of SVM on the Iris dataset, including data visualization, model training, evaluation, and hyperparameter tuning. Despite the small dataset size, the SVM model performs well, demonstrating the effectiveness of SVM for classification tasks.
