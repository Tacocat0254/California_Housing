<H1>California Housing Classification</H1>
This project analyzes and models the California Housing dataset to classify whether a housing block’s price is above the median using multiple machine learning models. The goal is to evaluate and compare different classifiers for binary classification and improve prediction performance using hyperparameter tuning.

<H2>Dataset</H2>
Source: california_housing.csv
Features:

- MedInc: Median income in block group
- HouseAge: Median house age
- AveRooms: Average number of rooms
- AveBedrms: Average number of bedrooms
- Population: Population of the block
- AveOccup: Average household occupancy
- Latitude, Longitude: Geo-coordinates
- price_above_median: Target (0 = below median, 1 = above median)

  <H2>Results Summary</H2>

| Model             | Accuracy | Precision | Recall | F1 Score |
| ----------------- | -------- | --------- | ------ | -------- |
| **KNN**           | 0.84     | 0.84      | 0.84   | 0.84     |
| **Decision Tree** | 0.85     | 0.85      | 0.85   | 0.85     |
| **Random Forest** | 0.89     | 0.89      | 0.89   | 0.89     |
| **AdaBoost**      | 0.89     | 0.89      | 0.89   | 0.89     |


<H2>Libraries Used</H2>

| Section                     | Libraries                                                                                                                                                         |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Data Handling**           | `pandas`, `numpy`                                                                                                                                                 |
| **Visualization**           | `matplotlib`, `seaborn`                                                                                                                                           |
| **Preprocessing & Scaling** | `sklearn.preprocessing.StandardScaler`, `sklearn.model_selection.train_test_split`                                                                                |
| **Modeling**                | `sklearn.neighbors.KNeighborsClassifier`, `sklearn.tree.DecisionTreeClassifier`, `sklearn.ensemble.RandomForestClassifier`, `sklearn.ensemble.AdaBoostClassifier` |
| **Model Tuning**            | `sklearn.model_selection.GridSearchCV`, `RandomizedSearchCV`                                                                                                      |
| **Evaluation**              | `sklearn.metrics` (`accuracy_score`, `precision_score`, `recall_score`, `f1_score`, `confusion_matrix`, `classification_report`)                                  |
