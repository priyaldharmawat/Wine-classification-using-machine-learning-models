# Wine Quality Classification

This repository contains the code for a machine learning project that classifies the quality of wine (red and white) based on various chemical properties. The project utilizes several classification algorithms, including K-Nearest Neighbors (KNN), Decision Tree, Random Forest, Gradient Boosting, and Neural Networks.

## Project Goals

*   Explore and analyze the Wine Quality dataset.
*   Build and evaluate machine learning models for wine quality classification.
*   Compare the performance of different models and identify the most effective one.

## Data

The dataset used in this project is the Wine Quality dataset from the UCI Machine Learning Repository. It combines red and white wine data and contains the following attributes:

*   **Fixed Acidity:** tartness of the wine.
*   **Volatile Acidity:** amount of acetic acid in wine.
*   **Citric Acid:** acts as a preservative and adds flavor.
*   **Residual Sugar:** amount of sugar remaining after fermentation.
*   **Chlorides:** amount of salt in the wine.
*   **Free Sulfur Dioxide:** prevents microbial growth and oxidation.
*   **Total Sulfur Dioxide:** total amount of SO2 in the wine.
*   **Density:** density of the wine.
*   **pH:** acidity level of the wine.
*   **Sulphates:** amount of sulfur added to the wine.
*   **Alcohol:** percentage of alcohol in the wine.
*   **Quality:** quality score between 0 and 10 (target variable).
*   **Wine:** Type of wine (red or white)

## Code

The core code is in the `wine_quality_classification.py` file. It performs the following steps:

1.  **Data Loading and Preprocessing:**
    *   Loads the data from `wine.csv`.
    *   Encodes the 'wine' categorical feature using Label Encoding.
    *   Splits the data into training (70%) and testing (30%) sets.
    *   Scales the features using StandardScaler.
2.  **Model Building and Evaluation:**
    *   **K-Nearest Neighbors (KNN):** Determines the optimal `k` value using cross-validation and plots an elbow curve.
    *   **Decision Tree:** Trains and evaluates a Decision Tree Classifier.
    *   **Random Forest:** Trains and evaluates a Random Forest Classifier.
    *   **Gradient Boosting:** Trains and evaluates a Gradient Boosting Classifier.
    *   **Neural Networks:**
        *   Trains and evaluates Multi-layer Perceptron (MLP) classifiers with 'adam' and 'sgd' solvers.
        *   Performs hyperparameter tuning using GridSearchCV to optimize the neural network architecture.
3.  **Model Comparison:**
    *   Compares the performance of all models based on accuracy, recall, and precision.
    *   Visualizes the results using a bar chart.

## Running the Code

1.  Install the required libraries: `pip install -r requirements.txt` (Create a `requirements.txt` file listing dependencies like `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`). Example:
    ```
    pandas
    numpy
    scikit-learn
    matplotlib
    seaborn
    statsmodels
    ```
2.  Run the script: `python wine_quality_classification.py`

## Results

The project found that the **Random Forest** model generally performed best in terms of accuracy, recall, and precision. The results are visualized in a bar chart within the script output. The optimal k value for KNN was found to be 1. The optimized Neural Network didn't show significant improvement over the basic Neural Network models.

Here's a summary of the best-performing models (replace with your actual results):

*   **Random Forest:**
    *   Accuracy: 0.673
    *   Recall: 0.673
    *   Precision: 0.674

## Future Work

*   Explore feature engineering to potentially improve model performance.
*   Investigate other classification algorithms.
*   Perform more extensive hyperparameter tuning for all models.
*   Analyze feature importance to understand which chemical properties most influence wine quality.
*   Consider using different evaluation metrics like F1-score.

## Author

Priyal Dharmawat

---

Feel free to explore and adapt this project to your needs. Happy coding! 🚀



