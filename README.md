# Bank-Note-Authentication-using-Classification-Algorithms-

## Banknote Authentication Using Classification Algorithms

### Aim

Develop and evaluate supervised‑learning models that accurately distinguish genuine banknotes from forgeries based on statistical features extracted with a wavelet transform.

### Objective

1. **Exploratory Data Analysis (EDA)** – understand feature distributions, detect outliers, and inspect class balance.
2. **Model building & evaluation** – train multiple classification algorithms, tune hyper‑parameters, and compare performance using cross‑validation and test‑set metrics (accuracy, precision‑recall, ROC‑AUC).
3. **Model interpretation** – identify the most influential features for each algorithm and visualise decision boundaries or feature importances.
4. **Deployment‑readiness** – save the best model as a pickled object for later inference and provide a lightweight prediction script/notebook.

### Context

Data were extracted from images that were taken from genuine and forged banknote-like specimens. For digitization, an industrial camera usually used for print inspection was used. The final images have 400x 400 pixels. Due to the object lens and distance to the investigated object gray-scale pictures with a resolution of about 660 dpi were gained. Wavelet Transform tool were used to extract features from images.

### Built using 
* Python

### Data‑Set Source & Features

| Item             | Description                                                                                                                                                                                                                                                                    |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Origin**       | [UCI Banknote Authentication Data Set](https://archive.ics.uci.edu/ml/datasets/banknote+authentication) – mirrored on Kaggle: [https://www.kaggle.com/datasets/shantanuss/banknote-authentication-uci](https://www.kaggle.com/datasets/shantanuss/banknote-authentication-uci) |
| **Observations** | 1 ,372 banknote specimens (genuine & forged)                                                                                                                                                                                                                                   |
| **Features**     | *variance*, *skewness*, *curtosis*, *entropy* (all continuous)                                                                                                                                                                                                                 |
| **Target**       | `class` – 0 = forged, 1 = genuine                                                                                                                                                                                                                                              |
| **Format**       | CSV, 5 columns, no missing values                                                                                                                                                                                                                                              |

### Libraries & Packages Used

| Purpose       | Package                                                                                              |
| ------------- | ---------------------------------------------------------------------------------------------------- |                                                             |
| Data handling | `pandas`, `scipy`                                                                                    |
| Visualisation | `matplotlib`, `seaborn`                                                                              |
| Modelling     | `scikit‑learn` (`LogisticRegression`, `DecisionTreeClassifier`, `RandomForestClassifier`), `xgboost` |

