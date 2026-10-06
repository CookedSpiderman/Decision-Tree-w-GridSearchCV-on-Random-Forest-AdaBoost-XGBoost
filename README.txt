Decision Trees - Assignment 2

Dataset:

This project uses the Raisin dataset from the UCI Machine Learning Repository (Dataset ID 850). The dataset is loaded directly in the notebook using the ucimlrepo Python package, so no local dataset file is required.

Models:

The notebook builds and evaluates the following classification models:

- Decision Tree
- Random Forest
- AdaBoost
- XGBoost

GridSearchCV with cross-validation is used to tune the hyperparameters of each model.

Required Libraries:

The notebook requires the following Python libraries:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost
- ucimlrepo

If any packages are missing, they can be installed using pip before running the notebook.

How to Run:

1. Open the .ipynb file using Jupyter Notebook, JupyterLab, or Google Colab.
2. Make sure the required Python libraries are installed.
3. Run the notebook cells from top to bottom in order.
4. The notebook will automatically download the Raisin dataset using ucimlrepo.
5. The notebook performs preprocessing, exploratory data analysis, model construction, hyperparameter tuning, and final model evaluation.

Execution Time:

The complete notebook may take more than 2 minutes to execute. The GridSearchCV sections, especially for Random Forest, AdaBoost, and XGBoost, test multiple hyperparameter combinations using cross-validation and therefore require more computation time.

Execution time will vary depending on the computer or environment being used. Please allow the GridSearchCV cells to finish before continuing to later cells.

Notes and Assumptions:

- The dataset is divided into training and testing sets using a fixed random state for reproducibility.
- Stratified sampling is used to maintain the equal distribution of Kecimen and Besni raisins between the training and testing sets.
- Standardization and normalization are demonstrated during preprocessing, although the original feature values are used for the tree-based models because tree algorithms are generally not sensitive to feature scale.
- Hyperparameters are selected using GridSearchCV and cross-validation on the training data.
- Final model performance is evaluated using accuracy, precision, recall, F1-score, confusion matrices, ROC curves, and Precision-Recall curves.