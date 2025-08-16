## Plant Growth Classification

### Project Overview

This project aims to classify **plant growth milestones** based on a variety of environmental factors. By analyzing features such as soil type, sunlight hours, water frequency, fertilizer type, temperature, and humidity, the goal is to develop a machine learning model that can predict a binary outcome for a significant growth milestone. This can be a valuable tool for agriculture, botany, and automated farming systems.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Plant Growth Data Classification](https://www.kaggle.com/datasets/gorororororo23/plant-growth-data-classification)
  * **Size**: 193 entries, 7 columns.
  * **Key Features**:
      * **Categorical**: Soil\_Type, Water\_Frequency, Fertilizer\_Type.
      * **Numerical**: Sunlight\_Hours, Temperature, Humidity.
  * **Approach**:
      * **Data Cleaning**: The dataset was clean with no missing values or duplicates. The class distribution is very balanced, with 97 entries for class 0 and 96 for class 1.
      * **Exploratory Data Analysis**: Histograms and boxplots were used to visualize the distribution of numerical features. Count plots were used for categorical features. A heatmap was generated to show the correlation between numerical features.
      * **Label Encoding**: Applied to all columns, including categorical features and the numerical features and the target Growth\_Milestone.
      * **Binary Classification**: The target variable Growth\_Milestone indicates a binary outcome (0 or 1).
      * **Models Used**:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * **59.0%** with Decision Tree Classifier.
      * **56.4%** with Random Forest and AdaBoost Classifiers.
      * Most models achieved moderate accuracies, suggesting that while some relationships exist, the task is challenging given the small dataset size and the complexity of plant growth.

-----

### Purpose and Applications

  * **Predict significant growth milestones for plants** in agricultural and botanical research.
  * Aid in optimizing growing conditions for different plant species.
  * Support data-driven decision-making in automated greenhouses and smart farming.
  * Serve as a foundational model for developing more advanced plant phenotyping systems.

-----

### Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Plant-Growth-Classification-Using-ML.git
cd Plant-Growth-Classification-Using-M
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Exploring more robust strategies for handling the very small dataset size, such as more extensive cross-validation techniques.
  * Investigating alternative encoding methods for categorical features and their impact.
  * Performing comprehensive hyperparameter tuning for all models.
  * Adding explainability (e.g., SHAP or LIME) to understand which environmental factors are the most influential for a plant's growth milestone.
